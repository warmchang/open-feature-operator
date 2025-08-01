# OpenFeature Operator

## TL;DR

> This helm chart has a dependency on [cert manager](https://cert-manager.io/docs/installation/)

```
helm repo add openfeature https://open-feature.github.io/open-feature-operator/
helm repo update
helm upgrade --install open-feature-operator openfeature/open-feature-operator
```

## Introduction

The OpenFeature Operator is a Kubernetes native operator that allows you to expose feature flags to your applications. It injects a [flagd](https://github.com/open-feature/flagd) sidecar into your pod and allows you to poll the flagd server for feature flags in a variety of ways.
The full documentation for this project can be found here: [OpenFeature Operator](https://github.com/open-feature/open-feature-operator/tree/main/docs)

## Prerequisites

The OpenFeature Operator requires [cert manager](https://cert-manager.io/docs/installation/) to be installed on the target cluster.

## Install

To install the chart with the release name `open-feature-operator`:

```
helm repo add openfeature https://open-feature.github.io/open-feature-operator/
helm repo update
helm upgrade --install open-feature-operator openfeature/open-feature-operator
```

This installation will use the default helm configuration, described in the [Configuration section](#configuration)
To overwrite these default values use the `--set` flag when calling `helm upgrade` or `helm install`, for example:

```
helm upgrade -i open-feature-operator ./chart/open-feature-operator --set sidecarConfiguration.port=8080 --set controllerManager.kubeRbacProxy.resources.limits.cpu=400m
```

## Upgrade

To install the chart with the release name `open-feature-operator`:

```sh
helm repo update
helm upgrade --install open-feature-operator openfeature/open-feature-operator
```

> [!NOTE]
> If you upgrade to OFO `v0.5.4` or higher while using a `flagd-proxy` provider, the instance of
`flagd-proxy` will be automatically upgraded to the latest supported version by the `open-feature-operator`.
The upgrade of `flagd-proxy` will also consider your current `FeatureFlagSource` configuration and adapt
the `flagd-proxy` Deployment accordingly.
If you are upgrading OFO to `v0.5.3` or lower, `flagd-proxy` (if present) won't be upgraded automatically.

#### Upgrade CRDs

CRDs are not upgraded automatically with helm (https://helm.sh/docs/chart_best_practices/custom_resource_definitions/).
OpenFeature Operator's CRDs are templated, and can be updated apart from the operator itself by using helm's template functionality and piping the output to `kubectl`:

```console
helm template openfeature/open-feature-operator -s templates/{CRD} | kubectl apply -f -
```

For the `featureflags.core.openfeature.dev` CRD:

```sh
helm template openfeature/open-feature-operator -s templates/apiextensions.k8s.io_v1_customresourcedefinition_featureflags.core.openfeature.dev.yaml | kubectl apply -f -
```

For the `featureflagsources.core.openfeature.dev` CRD:

```sh
helm template openfeature/open-feature-operator -s templates/apiextensions.k8s.io_v1_customresourcedefinition_featureflagsources.core.openfeature.dev.yaml | kubectl apply -f -
```

Keep in mind, you can set values as usual during this process:

```console
helm template openfeature/open-feature-operator -s templates/{CRD} --set defaultNamespace=myns | kubectl apply -f -
```

## Uninstall

To uninstall the `open-feature-operator`:

```
helm uninstall open-feature-operator
```

The command removes all the Kubernetes components associated with the chart and deletes the release.

## Configuration

### Global

| Name               | Description                                                                                                                                                                                                  | Value                          |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------ |
| `defaultNamespace` | To override the namespace use the `--namespace` flag. This default is provided to ensure that the kustomize build charts in `/templates` deploy correctly when no `namespace` is provided via the `-n` flag. | `open-feature-operator-system` |

### namespace

| Name                    | Description                                                                                                                                                                                                                               | Value  |
| ----------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------ |
| `namespace.create`      | Whether to create the namespace as part of this chart.                                                                                                                                                                                    | `true` |
| `namespace.labels`      | Labels for the namespace if created as part of the chart.                                                                                                                                                                                 | `{}`   |
| `namespace.annotations` | Annotations for the namespace if created as part of the chart.                                                                                                                                                                            | `{}`   |
| `imagePullSecrets`      | Array of ImagePullSecret objects containing credentials for images pulled by the operator (flagdProxyConfiguration.image, flagdConfiguration.image, controllerManager.manager.image). Example: imagePullSecrets: [{"name": "my-secret"}]  | `[]`   |
| `labels`                | Labels to apply to all of the pods in the operator.                                                                                                                                                                                       | `{}`   |
| `annotations`           | Annotations to apply to all of the pods in the operator.                                                                                                                                                                                  | `{}`   |

### Mutating Webhook configuration

| Name                             | Description                                               | Value    |
| -------------------------------- | --------------------------------------------------------- | -------- |
| `mutatingWebhook.failurePolicy`  | FailurePolicy when the webhook does not respond           | `Ignore` |
| `mutatingWebhook.objectSelector` | ObjectSelector on which pods the mutatingWebhook will run | `{}`     |

### Sidecar configuration

| Name                                             | Description                                                                                                                                                                                                                                                 | Value                        |
| ------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------- |
| `sidecarConfiguration.port`                      | Sets the value of the `XXX_PORT` environment variable for the injected sidecar.                                                                                                                                                                             | `8013`                       |
| `sidecarConfiguration.managementPort`            | Sets the value of the `XXX_MANAGEMENT_PORT` environment variable for the injected sidecar.                                                                                                                                                                  | `8014`                       |
| `sidecarConfiguration.socketPath`                | Sets the value of the `XXX_SOCKET_PATH` environment variable for the injected sidecar.                                                                                                                                                                      | `""`                         |
| `sidecarConfiguration.image.repository`          | Sets the image for the injected sidecar.                                                                                                                                                                                                                    | `ghcr.io/open-feature/flagd` |
| `sidecarConfiguration.image.tag`                 | Sets the version tag for the injected sidecar.                                                                                                                                                                                                              | `v0.12.4`                    |
| `sidecarConfiguration.providerArgs`              | Used to append arguments to the sidecar startup command. This value is a comma separated string of key values separated by '=', e.g. `key=value,key2=value2` results in the appending of `--sync-provider-args key=value --sync-provider-args key2=value2`. | `""`                         |
| `sidecarConfiguration.envVarPrefix`              | Sets the prefix for all environment variables set in the injected sidecar.                                                                                                                                                                                  | `FLAGD`                      |
| `sidecarConfiguration.defaultSyncProvider`       | Sets the value of the `XXX_SYNC_PROVIDER` environment variable for the injected sidecar container. There are 4 valid sync providers: `kubernetes`, `grpc`, `file` and `http`.                                                                               | `kubernetes`                 |
| `sidecarConfiguration.evaluator`                 | Sets the value of the `XXX_EVALUATOR` environment variable for the injected sidecar container.                                                                                                                                                              | `json`                       |
| `sidecarConfiguration.logFormat`                 | Sets the value of the `XXX_LOG_FORMAT` environment variable for the injected sidecar container. There are 2 valid log formats: `json` and `console`.                                                                                                        | `json`                       |
| `sidecarConfiguration.probesEnabled`             | Enable or Disable Liveness and Readiness probes of the flagd sidecar. When enabled, HTTP probes( paths - `/readyz`, `/healthz`) are set with an initial delay of 5 seconds.                                                                                 | `true`                       |
| `sidecarConfiguration.debugLogging`              | Controls the addition of the `--debug` flag to the container startup arguments.                                                                                                                                                                             | `false`                      |
| `sidecarConfiguration.otelCollectorUri`          | Otel exporter uri.                                                                                                                                                                                                                                          | `""`                         |
| `sidecarConfiguration.resources.limits.cpu`      | Sets cpu resource limits for kube-rbac-proxy.                                                                                                                                                                                                               | `500m`                       |
| `sidecarConfiguration.resources.limits.memory`   | Sets memory resource limits for kube-rbac-proxy.                                                                                                                                                                                                            | `64Mi`                       |
| `sidecarConfiguration.resources.requests.cpu`    | Sets cpu resource requests for kube-rbac-proxy.                                                                                                                                                                                                             | `200m`                       |
| `sidecarConfiguration.resources.requests.memory` | Sets memory resource requests for kube-rbac-proxy.                                                                                                                                                                                                          | `32Mi`                       |

### In-process configuration

| Name                                           | Description                                                                                       | Value       |
| ---------------------------------------------- | ------------------------------------------------------------------------------------------------- | ----------- |
| `inProcessConfiguration.port`                  | Sets the value of the `XXX_PORT` environment variable for the pod containers.                     | `8015`      |
| `inProcessConfiguration.host`                  | Sets the value of the `XXX_HOST` environment variable for the pod containers.                     | `localhost` |
| `inProcessConfiguration.socketPath`            | Sets the value of the `XXX_SOCKET_PATH` environment variable for the pod containers.              | `""`        |
| `inProcessConfiguration.tls`                   | Sets the value of the `XXX_TLS` environment variable for the pod containers.                      | `false`     |
| `inProcessConfiguration.offlineFlagSourcePath` | Sets the value of the `XXX_OFFLINE_FLAG_SOURCE_PATH` environment variable for the pod containers. | `""`        |
| `inProcessConfiguration.selector`              | Sets the value of the `XXX_SELECTOR` environment variable for the pod containers.                 | `""`        |
| `inProcessConfiguration.envVarPrefix`          | Sets the value of the `XXX_ENV_VAR_PREFIX` environment variable for the pod containers.           | `FLAGD`     |
| `inProcessConfiguration.cache.type`            | Sets the value of the `XXX_CACHE` environment variable for the pod containers.                    | `lru`       |
| `inProcessConfiguration.cache.size`            | Sets the value of the `XXX_CACHE_MAX_SIZE` environment variable for the pod containers.           | `1000`      |

### Flagd-proxy configuration

| Name                                       | Description                                                                     | Value                              |
| ------------------------------------------ | ------------------------------------------------------------------------------- | ---------------------------------- |
| `flagdProxyConfiguration.replicaCount`     | sets the number of replicas for the flagd-proxy deployment.                     | `1`                                |
| `flagdProxyConfiguration.port`             | Sets the port to expose the sync API on.                                        | `8015`                             |
| `flagdProxyConfiguration.managementPort`   | Sets the port to expose the management API on.                                  | `8016`                             |
| `flagdProxyConfiguration.image.repository` | Sets the image for the flagd-proxy deployment.                                  | `ghcr.io/open-feature/flagd-proxy` |
| `flagdProxyConfiguration.image.tag`        | Sets the tag for the flagd-proxy deployment.                                    | `v0.7.4`                           |
| `flagdProxyConfiguration.debugLogging`     | Controls the addition of the `--debug` flag to the container startup arguments. | `false`                            |

### Flagd configuration

| Name                                  | Description                                                                     | Value                        |
| ------------------------------------- | ------------------------------------------------------------------------------- | ---------------------------- |
| `flagdConfiguration.port`             | Sets the port to expose the flagd API on.                                       | `8013`                       |
| `flagdConfiguration.ofrepPort`        | Sets the port to expose the ofrep API on.                                       | `8016`                       |
| `flagdConfiguration.syncPort`         | Sets the port to expose the sync API on.                                        | `8015`                       |
| `flagdConfiguration.managementPort`   | Sets the port to expose the management API on.                                  | `8014`                       |
| `flagdConfiguration.image.repository` | Sets the image for the flagd deployment.                                        | `ghcr.io/open-feature/flagd` |
| `flagdConfiguration.image.tag`        | Sets the tag for the flagd deployment.                                          | `v0.12.4`                    |
| `flagdConfiguration.debugLogging`     | Controls the addition of the `--debug` flag to the container startup arguments. | `false`                      |

### Operator resource configuration

| Name                                                                      | Description                                                                                                      | Value                                        |
| ------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- | -------------------------------------------- |
| `controllerManager.manager.image.repository`                              | Sets the image for the operator.                                                                                 | `ghcr.io/open-feature/open-feature-operator` |
| `controllerManager.manager.image.tag`                                     | Sets the version tag for the operator.                                                                           | `v0.8.7`                                     |
| `controllerManager.manager.resources.limits.cpu`                          | Sets cpu resource limits for operator.                                                                           | `500m`                                       |
| `controllerManager.manager.resources.limits.memory`                       | Sets memory resource limits for operator.                                                                        | `128Mi`                                      |
| `controllerManager.manager.resources.requests.cpu`                        | Sets cpu resource requests for operator.                                                                         | `10m`                                        |
| `controllerManager.manager.resources.requests.memory`                     | Sets memory resource requests for operator.                                                                      | `64Mi`                                       |
| `controllerManager.manager.hostNetwork`                                   | Should the injector pods run on the host network (useful when using an alternate CNI in EKS)                     | `false`                                      |
| `controllerManager.manager.dnsPolicy`                                     | Pod DNS resolution scheme. Should be `ClusterFirstWithHostNet` if hostNetwork is true, `ClusterFirst` otherwise. | `ClusterFirst`                               |
| `controllerManager.replicas`                                              | Sets number of replicas of the OpenFeature operator pod.                                                         | `1`                                          |
| `managerConfig.flagsValidationEnabled`                                    | Enables the validating webhook for FeatureFlag CR.                                                               | `true`                                       |
| `managerConfig.controllerManagerConfigYaml.health.healthProbeBindAddress` | Sets the bind address for health probes.                                                                         | `:8081`                                      |
| `managerConfig.controllerManagerConfigYaml.metrics.bindAddress`           | Sets the bind address for metrics (combined with bindPort).                                                      | `127.0.0.1`                                  |
| `managerConfig.controllerManagerConfigYaml.metrics.bindPort`              | Sets the bind port for metrics.                                                                                  | `8080`                                       |
| `managerConfig.controllerManagerConfigYaml.webhook.port`                  | Sets the bind address for webhook.                                                                               | `9443`                                       |

