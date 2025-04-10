# API Reference

Packages:

- [core.openfeature.dev/v1beta1](#coreopenfeaturedevv1beta1)

# core.openfeature.dev/v1beta1

Resource Types:

- [FeatureFlag](#featureflag)

- [FeatureFlagSource](#featureflagsource)

- [Flagd](#flagd)

- [InProcessConfiguration](#inprocessconfiguration)




## FeatureFlag
<sup><sup>[↩ Parent](#coreopenfeaturedevv1beta1 )</sup></sup>






FeatureFlag is the Schema for the featureflags API

<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Description</th>
            <th>Required</th>
        </tr>
    </thead>
    <tbody><tr>
      <td><b>apiVersion</b></td>
      <td>string</td>
      <td>core.openfeature.dev/v1beta1</td>
      <td>true</td>
      </tr>
      <tr>
      <td><b>kind</b></td>
      <td>string</td>
      <td>FeatureFlag</td>
      <td>true</td>
      </tr>
      <tr>
      <td><b><a href="https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.20/#objectmeta-v1-meta">metadata</a></b></td>
      <td>object</td>
      <td>Refer to the Kubernetes API documentation for the fields of the `metadata` field.</td>
      <td>true</td>
      </tr><tr>
        <td><b><a href="#featureflagspec">spec</a></b></td>
        <td>object</td>
        <td>
          FeatureFlagSpec defines the desired state of FeatureFlag<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>status</b></td>
        <td>object</td>
        <td>
          FeatureFlagStatus defines the observed state of FeatureFlag<br/>
        </td>
        <td>false</td>
      </tr></tbody>
</table>


### FeatureFlag.spec
<sup><sup>[↩ Parent](#featureflag)</sup></sup>



FeatureFlagSpec defines the desired state of FeatureFlag

<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Description</th>
            <th>Required</th>
        </tr>
    </thead>
    <tbody><tr>
        <td><b><a href="#featureflagspecflagspec">flagSpec</a></b></td>
        <td>object</td>
        <td>
          FlagSpec is the structured representation of the feature flag specification<br/>
        </td>
        <td>false</td>
      </tr></tbody>
</table>


### FeatureFlag.spec.flagSpec
<sup><sup>[↩ Parent](#featureflagspec)</sup></sup>



FlagSpec is the structured representation of the feature flag specification

<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Description</th>
            <th>Required</th>
        </tr>
    </thead>
    <tbody><tr>
        <td><b><a href="#featureflagspecflagspecflagskey">flags</a></b></td>
        <td>map[string]object</td>
        <td>
          <br/>
        </td>
        <td>true</td>
      </tr><tr>
        <td><b>$evaluators</b></td>
        <td>object</td>
        <td>
          <br/>
        </td>
        <td>false</td>
      </tr></tbody>
</table>


### FeatureFlag.spec.flagSpec.flags[key]
<sup><sup>[↩ Parent](#featureflagspecflagspec)</sup></sup>





<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Description</th>
            <th>Required</th>
        </tr>
    </thead>
    <tbody><tr>
        <td><b>defaultVariant</b></td>
        <td>string</td>
        <td>
          <br/>
        </td>
        <td>true</td>
      </tr><tr>
        <td><b>state</b></td>
        <td>enum</td>
        <td>
          <br/>
          <br/>
            <i>Enum</i>: ENABLED, DISABLED<br/>
        </td>
        <td>true</td>
      </tr><tr>
        <td><b>variants</b></td>
        <td>object</td>
        <td>
          <br/>
        </td>
        <td>true</td>
      </tr><tr>
        <td><b>targeting</b></td>
        <td>object</td>
        <td>
          Targeting is the json targeting rule<br/>
        </td>
        <td>false</td>
      </tr></tbody>
</table>

## FeatureFlagSource
<sup><sup>[↩ Parent](#coreopenfeaturedevv1beta1 )</sup></sup>






FeatureFlagSource is the Schema for the FeatureFlagSources API

<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Description</th>
            <th>Required</th>
        </tr>
    </thead>
    <tbody><tr>
      <td><b>apiVersion</b></td>
      <td>string</td>
      <td>core.openfeature.dev/v1beta1</td>
      <td>true</td>
      </tr>
      <tr>
      <td><b>kind</b></td>
      <td>string</td>
      <td>FeatureFlagSource</td>
      <td>true</td>
      </tr>
      <tr>
      <td><b><a href="https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.20/#objectmeta-v1-meta">metadata</a></b></td>
      <td>object</td>
      <td>Refer to the Kubernetes API documentation for the fields of the `metadata` field.</td>
      <td>true</td>
      </tr><tr>
        <td><b><a href="#featureflagsourcespec">spec</a></b></td>
        <td>object</td>
        <td>
          FeatureFlagSourceSpec defines the desired state of FeatureFlagSource<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>status</b></td>
        <td>object</td>
        <td>
          FeatureFlagSourceStatus defines the observed state of FeatureFlagSource<br/>
        </td>
        <td>false</td>
      </tr></tbody>
</table>


### FeatureFlagSource.spec
<sup><sup>[↩ Parent](#featureflagsource)</sup></sup>



FeatureFlagSourceSpec defines the desired state of FeatureFlagSource

<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Description</th>
            <th>Required</th>
        </tr>
    </thead>
    <tbody><tr>
        <td><b><a href="#featureflagsourcespecsourcesindex">sources</a></b></td>
        <td>[]object</td>
        <td>
          SyncProviders define the syncProviders and associated configuration to be applied to the sidecar<br/>
        </td>
        <td>true</td>
      </tr><tr>
        <td><b>debugLogging</b></td>
        <td>boolean</td>
        <td>
          DebugLogging defines whether to enable --debug flag of flagd sidecar. Default false (disabled).<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>defaultSyncProvider</b></td>
        <td>string</td>
        <td>
          DefaultSyncProvider defines the default sync provider<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>envVarPrefix</b></td>
        <td>string</td>
        <td>
          EnvVarPrefix defines the prefix to be applied to all environment variables applied to the sidecar, default FLAGD<br/>
          <br/>
            <i>Default</i>: FLAGD<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b><a href="#featureflagsourcespecenvvarsindex">envVars</a></b></td>
        <td>[]object</td>
        <td>
          EnvVars define the env vars to be applied to the sidecar, any env vars in FeatureFlag CRs
are added at the lowest index, all values will have the EnvVarPrefix applied, default FLAGD<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>evaluator</b></td>
        <td>string</td>
        <td>
          Evaluator sets an evaluator, defaults to 'json'<br/>
          <br/>
            <i>Default</i>: json<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>logFormat</b></td>
        <td>string</td>
        <td>
          LogFormat allows for the sidecar log format to be overridden, defaults to 'json'<br/>
          <br/>
            <i>Default</i>: json<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>managementPort</b></td>
        <td>integer</td>
        <td>
          ManagemetPort defines the port to serve management on, defaults to 8014<br/>
          <br/>
            <i>Format</i>: int32<br/>
            <i>Default</i>: 8014<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>otelCollectorUri</b></td>
        <td>string</td>
        <td>
          OtelCollectorUri defines whether to enable --otel-collector-uri flag of flagd sidecar. Default false (disabled).<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>port</b></td>
        <td>integer</td>
        <td>
          Port defines the port to listen on, defaults to 8013<br/>
          <br/>
            <i>Format</i>: int32<br/>
            <i>Default</i>: 8013<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>probesEnabled</b></td>
        <td>boolean</td>
        <td>
          ProbesEnabled defines whether to enable liveness and readiness probes of flagd sidecar. Default true (enabled).<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b><a href="#featureflagsourcespecresources">resources</a></b></td>
        <td>object</td>
        <td>
          Resources defines flagd sidecar resources. Default to operator sidecar-cpu-* and sidecar-ram-* flags.<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>rolloutOnChange</b></td>
        <td>boolean</td>
        <td>
          RolloutOnChange dictates whether annotated deployments will be restarted when configuration changes are
detected in this CR, defaults to false<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>socketPath</b></td>
        <td>string</td>
        <td>
          SocketPath defines the unix socket path to listen on<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>syncProviderArgs</b></td>
        <td>[]string</td>
        <td>
          SyncProviderArgs are string arguments passed to all sync providers, defined as key values separated by =<br/>
        </td>
        <td>false</td>
      </tr></tbody>
</table>


### FeatureFlagSource.spec.sources[index]
<sup><sup>[↩ Parent](#featureflagsourcespec)</sup></sup>





<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Description</th>
            <th>Required</th>
        </tr>
    </thead>
    <tbody><tr>
        <td><b>source</b></td>
        <td>string</td>
        <td>
          Source is a URI of the flag sources<br/>
        </td>
        <td>true</td>
      </tr><tr>
        <td><b>certPath</b></td>
        <td>string</td>
        <td>
          CertPath is a path of a certificate to be used by grpc TLS connection<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>httpSyncBearerToken</b></td>
        <td>string</td>
        <td>
          HttpSyncBearerToken is a bearer token. Used by http(s) sync provider only<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>interval</b></td>
        <td>integer</td>
        <td>
          Interval is a flag configuration interval in seconds used by http provider<br/>
          <br/>
            <i>Format</i>: int32<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>provider</b></td>
        <td>string</td>
        <td>
          Provider type - kubernetes, http(s), grpc(s) or file<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>providerID</b></td>
        <td>string</td>
        <td>
          ProviderID is an identifier to be used in grpc provider<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>selector</b></td>
        <td>string</td>
        <td>
          Selector is a flag configuration selector used by grpc provider<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>tls</b></td>
        <td>boolean</td>
        <td>
          TLS - Enable/Disable secure TLS connectivity. Currently used only by GRPC sync<br/>
        </td>
        <td>false</td>
      </tr></tbody>
</table>


### FeatureFlagSource.spec.envVars[index]
<sup><sup>[↩ Parent](#featureflagsourcespec)</sup></sup>



EnvVar represents an environment variable present in a Container.

<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Description</th>
            <th>Required</th>
        </tr>
    </thead>
    <tbody><tr>
        <td><b>name</b></td>
        <td>string</td>
        <td>
          Name of the environment variable. Must be a C&lowbar;IDENTIFIER.<br/>
        </td>
        <td>true</td>
      </tr><tr>
        <td><b>value</b></td>
        <td>string</td>
        <td>
          Variable references $(VAR&lowbar;NAME) are expanded
using the previously defined environment variables in the container and
any service environment variables. If a variable cannot be resolved,
the reference in the input string will be unchanged. Double $$ are reduced
to a single $, which allows for escaping the $(VAR&lowbar;NAME) syntax: i.e.
"$$(VAR&lowbar;NAME)" will produce the string literal "$(VAR&lowbar;NAME)".
Escaped references will never be expanded, regardless of whether the variable
exists or not.
Defaults to "".<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b><a href="#featureflagsourcespecenvvarsindexvaluefrom">valueFrom</a></b></td>
        <td>object</td>
        <td>
          Source for the environment variable's value. Cannot be used if value is not empty.<br/>
        </td>
        <td>false</td>
      </tr></tbody>
</table>


### FeatureFlagSource.spec.envVars[index].valueFrom
<sup><sup>[↩ Parent](#featureflagsourcespecenvvarsindex)</sup></sup>



Source for the environment variable's value. Cannot be used if value is not empty.

<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Description</th>
            <th>Required</th>
        </tr>
    </thead>
    <tbody><tr>
        <td><b><a href="#featureflagsourcespecenvvarsindexvaluefromconfigmapkeyref">configMapKeyRef</a></b></td>
        <td>object</td>
        <td>
          Selects a key of a ConfigMap.<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b><a href="#featureflagsourcespecenvvarsindexvaluefromfieldref">fieldRef</a></b></td>
        <td>object</td>
        <td>
          Selects a field of the pod: supports metadata.name, metadata.namespace, `metadata.labels['&lt;KEY&gt;']`, `metadata.annotations['&lt;KEY&gt;']`,
spec.nodeName, spec.serviceAccountName, status.hostIP, status.podIP, status.podIPs.<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b><a href="#featureflagsourcespecenvvarsindexvaluefromresourcefieldref">resourceFieldRef</a></b></td>
        <td>object</td>
        <td>
          Selects a resource of the container: only resources limits and requests
(limits.cpu, limits.memory, limits.ephemeral-storage, requests.cpu, requests.memory and requests.ephemeral-storage) are currently supported.<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b><a href="#featureflagsourcespecenvvarsindexvaluefromsecretkeyref">secretKeyRef</a></b></td>
        <td>object</td>
        <td>
          Selects a key of a secret in the pod's namespace<br/>
        </td>
        <td>false</td>
      </tr></tbody>
</table>


### FeatureFlagSource.spec.envVars[index].valueFrom.configMapKeyRef
<sup><sup>[↩ Parent](#featureflagsourcespecenvvarsindexvaluefrom)</sup></sup>



Selects a key of a ConfigMap.

<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Description</th>
            <th>Required</th>
        </tr>
    </thead>
    <tbody><tr>
        <td><b>key</b></td>
        <td>string</td>
        <td>
          The key to select.<br/>
        </td>
        <td>true</td>
      </tr><tr>
        <td><b>name</b></td>
        <td>string</td>
        <td>
          Name of the referent.
This field is effectively required, but due to backwards compatibility is
allowed to be empty. Instances of this type with an empty value here are
almost certainly wrong.
More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names<br/>
          <br/>
            <i>Default</i>: <br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>optional</b></td>
        <td>boolean</td>
        <td>
          Specify whether the ConfigMap or its key must be defined<br/>
        </td>
        <td>false</td>
      </tr></tbody>
</table>


### FeatureFlagSource.spec.envVars[index].valueFrom.fieldRef
<sup><sup>[↩ Parent](#featureflagsourcespecenvvarsindexvaluefrom)</sup></sup>



Selects a field of the pod: supports metadata.name, metadata.namespace, `metadata.labels['&lt;KEY&gt;']`, `metadata.annotations['&lt;KEY&gt;']`,
spec.nodeName, spec.serviceAccountName, status.hostIP, status.podIP, status.podIPs.

<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Description</th>
            <th>Required</th>
        </tr>
    </thead>
    <tbody><tr>
        <td><b>fieldPath</b></td>
        <td>string</td>
        <td>
          Path of the field to select in the specified API version.<br/>
        </td>
        <td>true</td>
      </tr><tr>
        <td><b>apiVersion</b></td>
        <td>string</td>
        <td>
          Version of the schema the FieldPath is written in terms of, defaults to "v1".<br/>
        </td>
        <td>false</td>
      </tr></tbody>
</table>


### FeatureFlagSource.spec.envVars[index].valueFrom.resourceFieldRef
<sup><sup>[↩ Parent](#featureflagsourcespecenvvarsindexvaluefrom)</sup></sup>



Selects a resource of the container: only resources limits and requests
(limits.cpu, limits.memory, limits.ephemeral-storage, requests.cpu, requests.memory and requests.ephemeral-storage) are currently supported.

<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Description</th>
            <th>Required</th>
        </tr>
    </thead>
    <tbody><tr>
        <td><b>resource</b></td>
        <td>string</td>
        <td>
          Required: resource to select<br/>
        </td>
        <td>true</td>
      </tr><tr>
        <td><b>containerName</b></td>
        <td>string</td>
        <td>
          Container name: required for volumes, optional for env vars<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>divisor</b></td>
        <td>int or string</td>
        <td>
          Specifies the output format of the exposed resources, defaults to "1"<br/>
        </td>
        <td>false</td>
      </tr></tbody>
</table>


### FeatureFlagSource.spec.envVars[index].valueFrom.secretKeyRef
<sup><sup>[↩ Parent](#featureflagsourcespecenvvarsindexvaluefrom)</sup></sup>



Selects a key of a secret in the pod's namespace

<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Description</th>
            <th>Required</th>
        </tr>
    </thead>
    <tbody><tr>
        <td><b>key</b></td>
        <td>string</td>
        <td>
          The key of the secret to select from.  Must be a valid secret key.<br/>
        </td>
        <td>true</td>
      </tr><tr>
        <td><b>name</b></td>
        <td>string</td>
        <td>
          Name of the referent.
This field is effectively required, but due to backwards compatibility is
allowed to be empty. Instances of this type with an empty value here are
almost certainly wrong.
More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names<br/>
          <br/>
            <i>Default</i>: <br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>optional</b></td>
        <td>boolean</td>
        <td>
          Specify whether the Secret or its key must be defined<br/>
        </td>
        <td>false</td>
      </tr></tbody>
</table>


### FeatureFlagSource.spec.resources
<sup><sup>[↩ Parent](#featureflagsourcespec)</sup></sup>



Resources defines flagd sidecar resources. Default to operator sidecar-cpu-* and sidecar-ram-* flags.

<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Description</th>
            <th>Required</th>
        </tr>
    </thead>
    <tbody><tr>
        <td><b><a href="#featureflagsourcespecresourcesclaimsindex">claims</a></b></td>
        <td>[]object</td>
        <td>
          Claims lists the names of resources, defined in spec.resourceClaims,
that are used by this container.

This is an alpha field and requires enabling the
DynamicResourceAllocation feature gate.

This field is immutable. It can only be set for containers.<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>limits</b></td>
        <td>map[string]int or string</td>
        <td>
          Limits describes the maximum amount of compute resources allowed.
More info: https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>requests</b></td>
        <td>map[string]int or string</td>
        <td>
          Requests describes the minimum amount of compute resources required.
If Requests is omitted for a container, it defaults to Limits if that is explicitly specified,
otherwise to an implementation-defined value. Requests cannot exceed Limits.
More info: https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/<br/>
        </td>
        <td>false</td>
      </tr></tbody>
</table>


### FeatureFlagSource.spec.resources.claims[index]
<sup><sup>[↩ Parent](#featureflagsourcespecresources)</sup></sup>



ResourceClaim references one entry in PodSpec.ResourceClaims.

<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Description</th>
            <th>Required</th>
        </tr>
    </thead>
    <tbody><tr>
        <td><b>name</b></td>
        <td>string</td>
        <td>
          Name must match the name of one entry in pod.spec.resourceClaims of
the Pod where this field is used. It makes that resource available
inside a container.<br/>
        </td>
        <td>true</td>
      </tr><tr>
        <td><b>request</b></td>
        <td>string</td>
        <td>
          Request is the name chosen for a request in the referenced claim.
If empty, everything from the claim is made available, otherwise
only the result of this request.<br/>
        </td>
        <td>false</td>
      </tr></tbody>
</table>

## Flagd
<sup><sup>[↩ Parent](#coreopenfeaturedevv1beta1 )</sup></sup>






Flagd is the Schema for the flagds API

<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Description</th>
            <th>Required</th>
        </tr>
    </thead>
    <tbody><tr>
      <td><b>apiVersion</b></td>
      <td>string</td>
      <td>core.openfeature.dev/v1beta1</td>
      <td>true</td>
      </tr>
      <tr>
      <td><b>kind</b></td>
      <td>string</td>
      <td>Flagd</td>
      <td>true</td>
      </tr>
      <tr>
      <td><b><a href="https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.20/#objectmeta-v1-meta">metadata</a></b></td>
      <td>object</td>
      <td>Refer to the Kubernetes API documentation for the fields of the `metadata` field.</td>
      <td>true</td>
      </tr><tr>
        <td><b><a href="#flagdspec">spec</a></b></td>
        <td>object</td>
        <td>
          FlagdSpec defines the desired state of Flagd<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>status</b></td>
        <td>object</td>
        <td>
          FlagdStatus defines the observed state of Flagd<br/>
        </td>
        <td>false</td>
      </tr></tbody>
</table>


### Flagd.spec
<sup><sup>[↩ Parent](#flagd)</sup></sup>



FlagdSpec defines the desired state of Flagd

<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Description</th>
            <th>Required</th>
        </tr>
    </thead>
    <tbody><tr>
        <td><b>featureFlagSource</b></td>
        <td>string</td>
        <td>
          FeatureFlagSource references to a FeatureFlagSource from which the created flagd instance retrieves
the feature flag configurations<br/>
        </td>
        <td>true</td>
      </tr><tr>
        <td><b><a href="#flagdspecgatewayapiroutes">gatewayApiRoutes</a></b></td>
        <td>object</td>
        <td>
          GatewayApiRoutes<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b><a href="#flagdspecingress">ingress</a></b></td>
        <td>object</td>
        <td>
          Ingress<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>replicas</b></td>
        <td>integer</td>
        <td>
          Replicas defines the number of replicas to create for the service.
Default: 1<br/>
          <br/>
            <i>Format</i>: int32<br/>
            <i>Default</i>: 1<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>serviceAccountName</b></td>
        <td>string</td>
        <td>
          ServiceAccountName the service account name for the flagd deployment<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>serviceType</b></td>
        <td>enum</td>
        <td>
          ServiceType represents the type of Service to create.
Must be one of: ClusterIP, NodePort, LoadBalancer, and ExternalName.
Default: ClusterIP<br/>
          <br/>
            <i>Enum</i>: ClusterIP, NodePort, LoadBalancer, ExternalName<br/>
            <i>Default</i>: ClusterIP<br/>
        </td>
        <td>false</td>
      </tr></tbody>
</table>


### Flagd.spec.gatewayApiRoutes
<sup><sup>[↩ Parent](#flagdspec)</sup></sup>



GatewayApiRoutes

<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Description</th>
            <th>Required</th>
        </tr>
    </thead>
    <tbody><tr>
        <td><b><a href="#flagdspecgatewayapiroutesparentrefsindex">parentRefs</a></b></td>
        <td>[]object</td>
        <td>
          ParentRefs references the resources (usually Gateways) that the Routes should
be attached to.<br/>
        </td>
        <td>true</td>
      </tr><tr>
        <td><b>annotations</b></td>
        <td>map[string]string</td>
        <td>
          Annotations to be added to the Gateway API routes<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>enabled</b></td>
        <td>boolean</td>
        <td>
          Enabled enables/disables the Gateway API routes for flagd<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>hosts</b></td>
        <td>[]string</td>
        <td>
          Hosts list of hosts to be added to the ingress.
Empty string corresponds to rule with no host.<br/>
        </td>
        <td>false</td>
      </tr></tbody>
</table>


### Flagd.spec.gatewayApiRoutes.parentRefs[index]
<sup><sup>[↩ Parent](#flagdspecgatewayapiroutes)</sup></sup>



ParentReference identifies an API object (usually a Gateway) that can be considered
a parent of this resource (usually a route). There are two kinds of parent resources
with "Core" support:

* Gateway (Gateway conformance profile)
* Service (Mesh conformance profile, ClusterIP Services only)

This API may be extended in the future to support additional kinds of parent
resources.

The API object must be valid in the cluster; the Group and Kind must
be registered in the cluster for this reference to be valid.

<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Description</th>
            <th>Required</th>
        </tr>
    </thead>
    <tbody><tr>
        <td><b>name</b></td>
        <td>string</td>
        <td>
          Name is the name of the referent.

Support: Core<br/>
        </td>
        <td>true</td>
      </tr><tr>
        <td><b>group</b></td>
        <td>string</td>
        <td>
          Group is the group of the referent.
When unspecified, "gateway.networking.k8s.io" is inferred.
To set the core API group (such as for a "Service" kind referent),
Group must be explicitly set to "" (empty string).

Support: Core<br/>
          <br/>
            <i>Default</i>: gateway.networking.k8s.io<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>kind</b></td>
        <td>string</td>
        <td>
          Kind is kind of the referent.

There are two kinds of parent resources with "Core" support:

* Gateway (Gateway conformance profile)
* Service (Mesh conformance profile, ClusterIP Services only)

Support for other resources is Implementation-Specific.<br/>
          <br/>
            <i>Default</i>: Gateway<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>namespace</b></td>
        <td>string</td>
        <td>
          Namespace is the namespace of the referent. When unspecified, this refers
to the local namespace of the Route.

Note that there are specific rules for ParentRefs which cross namespace
boundaries. Cross-namespace references are only valid if they are explicitly
allowed by something in the namespace they are referring to. For example:
Gateway has the AllowedRoutes field, and ReferenceGrant provides a
generic way to enable any other kind of cross-namespace reference.

&lt;gateway:experimental:description&gt;
ParentRefs from a Route to a Service in the same namespace are "producer"
routes, which apply default routing rules to inbound connections from
any namespace to the Service.

ParentRefs from a Route to a Service in a different namespace are
"consumer" routes, and these routing rules are only applied to outbound
connections originating from the same namespace as the Route, for which
the intended destination of the connections are a Service targeted as a
ParentRef of the Route.
&lt;/gateway:experimental:description&gt;

Support: Core<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>port</b></td>
        <td>integer</td>
        <td>
          Port is the network port this Route targets. It can be interpreted
differently based on the type of parent resource.

When the parent resource is a Gateway, this targets all listeners
listening on the specified port that also support this kind of Route(and
select this Route). It's not recommended to set `Port` unless the
networking behaviors specified in a Route must apply to a specific port
as opposed to a listener(s) whose port(s) may be changed. When both Port
and SectionName are specified, the name and port of the selected listener
must match both specified values.

&lt;gateway:experimental:description&gt;
When the parent resource is a Service, this targets a specific port in the
Service spec. When both Port (experimental) and SectionName are specified,
the name and port of the selected port must match both specified values.
&lt;/gateway:experimental:description&gt;

Implementations MAY choose to support other parent resources.
Implementations supporting other types of parent resources MUST clearly
document how/if Port is interpreted.

For the purpose of status, an attachment is considered successful as
long as the parent resource accepts it partially. For example, Gateway
listeners can restrict which Routes can attach to them by Route kind,
namespace, or hostname. If 1 of 2 Gateway listeners accept attachment
from the referencing Route, the Route MUST be considered successfully
attached. If no Gateway listeners accept attachment from this Route,
the Route MUST be considered detached from the Gateway.

Support: Extended<br/>
          <br/>
            <i>Format</i>: int32<br/>
            <i>Minimum</i>: 1<br/>
            <i>Maximum</i>: 65535<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>sectionName</b></td>
        <td>string</td>
        <td>
          SectionName is the name of a section within the target resource. In the
following resources, SectionName is interpreted as the following:

* Gateway: Listener name. When both Port (experimental) and SectionName
are specified, the name and port of the selected listener must match
both specified values.
* Service: Port name. When both Port (experimental) and SectionName
are specified, the name and port of the selected listener must match
both specified values.

Implementations MAY choose to support attaching Routes to other resources.
If that is the case, they MUST clearly document how SectionName is
interpreted.

When unspecified (empty string), this will reference the entire resource.
For the purpose of status, an attachment is considered successful if at
least one section in the parent resource accepts it. For example, Gateway
listeners can restrict which Routes can attach to them by Route kind,
namespace, or hostname. If 1 of 2 Gateway listeners accept attachment from
the referencing Route, the Route MUST be considered successfully
attached. If no Gateway listeners accept attachment from this Route, the
Route MUST be considered detached from the Gateway.

Support: Core<br/>
        </td>
        <td>false</td>
      </tr></tbody>
</table>


### Flagd.spec.ingress
<sup><sup>[↩ Parent](#flagdspec)</sup></sup>



Ingress

<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Description</th>
            <th>Required</th>
        </tr>
    </thead>
    <tbody><tr>
        <td><b>hosts</b></td>
        <td>[]string</td>
        <td>
          Hosts list of hosts to be added to the ingress.
Empty string corresponds to rule with no host.<br/>
        </td>
        <td>true</td>
      </tr><tr>
        <td><b>annotations</b></td>
        <td>map[string]string</td>
        <td>
          Annotations the annotations to be added to the ingress<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>enabled</b></td>
        <td>boolean</td>
        <td>
          Enabled enables/disables the ingress for flagd<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>flagdPath</b></td>
        <td>string</td>
        <td>
          FlagdPath is the path to be used for accessing the flagd flag evaluation API
Default: /flagd.evaluation.v1.Service<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>ingressClassName</b></td>
        <td>string</td>
        <td>
          IngressClassName defines the name if the ingress class to be used for flagd<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>ofrepPath</b></td>
        <td>string</td>
        <td>
          OFREPPath is the path to be used for accessing the OFREP API
Default: /ofrep<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>pathType</b></td>
        <td>string</td>
        <td>
          PathType is the path type to be used for the ingress rules<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>syncPath</b></td>
        <td>string</td>
        <td>
          SyncPath is the path to be used for accessing the sync API
Default: /flagd.sync.v1.Service<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b><a href="#flagdspecingresstlsindex">tls</a></b></td>
        <td>[]object</td>
        <td>
          TLS configuration for the ingress<br/>
        </td>
        <td>false</td>
      </tr></tbody>
</table>


### Flagd.spec.ingress.tls[index]
<sup><sup>[↩ Parent](#flagdspecingress)</sup></sup>



IngressTLS describes the transport layer security associated with an ingress.

<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Description</th>
            <th>Required</th>
        </tr>
    </thead>
    <tbody><tr>
        <td><b>hosts</b></td>
        <td>[]string</td>
        <td>
          hosts is a list of hosts included in the TLS certificate. The values in
this list must match the name/s used in the tlsSecret. Defaults to the
wildcard host setting for the loadbalancer controller fulfilling this
Ingress, if left unspecified.<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>secretName</b></td>
        <td>string</td>
        <td>
          secretName is the name of the secret used to terminate TLS traffic on
port 443. Field is left optional to allow TLS routing based on SNI
hostname alone. If the SNI host in a listener conflicts with the "Host"
header field used by an IngressRule, the SNI host is used for termination
and value of the "Host" header is used for routing.<br/>
        </td>
        <td>false</td>
      </tr></tbody>
</table>

## InProcessConfiguration
<sup><sup>[↩ Parent](#coreopenfeaturedevv1beta1 )</sup></sup>






InProcessConfiguration is the Schema for the inprocesconfigurations API

<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Description</th>
            <th>Required</th>
        </tr>
    </thead>
    <tbody><tr>
      <td><b>apiVersion</b></td>
      <td>string</td>
      <td>core.openfeature.dev/v1beta1</td>
      <td>true</td>
      </tr>
      <tr>
      <td><b>kind</b></td>
      <td>string</td>
      <td>InProcessConfiguration</td>
      <td>true</td>
      </tr>
      <tr>
      <td><b><a href="https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.20/#objectmeta-v1-meta">metadata</a></b></td>
      <td>object</td>
      <td>Refer to the Kubernetes API documentation for the fields of the `metadata` field.</td>
      <td>true</td>
      </tr><tr>
        <td><b><a href="#inprocessconfigurationspec">spec</a></b></td>
        <td>object</td>
        <td>
          InProcessConfigurationSpec defines the desired state of InProcessConfiguration<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>status</b></td>
        <td>object</td>
        <td>
          InProcessConfigurationStatus defines the observed state of InProcessConfiguration<br/>
        </td>
        <td>false</td>
      </tr></tbody>
</table>


### InProcessConfiguration.spec
<sup><sup>[↩ Parent](#inprocessconfiguration)</sup></sup>



InProcessConfigurationSpec defines the desired state of InProcessConfiguration

<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Description</th>
            <th>Required</th>
        </tr>
    </thead>
    <tbody><tr>
        <td><b>cache</b></td>
        <td>string</td>
        <td>
          Cache<br/>
          <br/>
            <i>Default</i>: lru<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>cacheMaxSize</b></td>
        <td>integer</td>
        <td>
          CacheMaxSize<br/>
          <br/>
            <i>Default</i>: 1000<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>envVarPrefix</b></td>
        <td>string</td>
        <td>
          EnvVarPrefix defines the prefix to be applied to all environment variables applied to the sidecar, default FLAGD<br/>
          <br/>
            <i>Default</i>: FLAGD<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b><a href="#inprocessconfigurationspecenvvarsindex">envVars</a></b></td>
        <td>[]object</td>
        <td>
          EnvVars<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>host</b></td>
        <td>string</td>
        <td>
          Host<br/>
          <br/>
            <i>Default</i>: localhost<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>offlineFlagSourcePath</b></td>
        <td>string</td>
        <td>
          OfflineFlagSourcePath<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>port</b></td>
        <td>integer</td>
        <td>
          Port defines the port to listen on, defaults to 8015<br/>
          <br/>
            <i>Format</i>: int32<br/>
            <i>Default</i>: 8015<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>selector</b></td>
        <td>string</td>
        <td>
          Selector<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>socketPath</b></td>
        <td>string</td>
        <td>
          SocketPath defines the unix socket path to listen on<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>tls</b></td>
        <td>boolean</td>
        <td>
          TLS<br/>
          <br/>
            <i>Default</i>: false<br/>
        </td>
        <td>false</td>
      </tr></tbody>
</table>


### InProcessConfiguration.spec.envVars[index]
<sup><sup>[↩ Parent](#inprocessconfigurationspec)</sup></sup>



EnvVar represents an environment variable present in a Container.

<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Description</th>
            <th>Required</th>
        </tr>
    </thead>
    <tbody><tr>
        <td><b>name</b></td>
        <td>string</td>
        <td>
          Name of the environment variable. Must be a C&lowbar;IDENTIFIER.<br/>
        </td>
        <td>true</td>
      </tr><tr>
        <td><b>value</b></td>
        <td>string</td>
        <td>
          Variable references $(VAR&lowbar;NAME) are expanded
using the previously defined environment variables in the container and
any service environment variables. If a variable cannot be resolved,
the reference in the input string will be unchanged. Double $$ are reduced
to a single $, which allows for escaping the $(VAR&lowbar;NAME) syntax: i.e.
"$$(VAR&lowbar;NAME)" will produce the string literal "$(VAR&lowbar;NAME)".
Escaped references will never be expanded, regardless of whether the variable
exists or not.
Defaults to "".<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b><a href="#inprocessconfigurationspecenvvarsindexvaluefrom">valueFrom</a></b></td>
        <td>object</td>
        <td>
          Source for the environment variable's value. Cannot be used if value is not empty.<br/>
        </td>
        <td>false</td>
      </tr></tbody>
</table>


### InProcessConfiguration.spec.envVars[index].valueFrom
<sup><sup>[↩ Parent](#inprocessconfigurationspecenvvarsindex)</sup></sup>



Source for the environment variable's value. Cannot be used if value is not empty.

<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Description</th>
            <th>Required</th>
        </tr>
    </thead>
    <tbody><tr>
        <td><b><a href="#inprocessconfigurationspecenvvarsindexvaluefromconfigmapkeyref">configMapKeyRef</a></b></td>
        <td>object</td>
        <td>
          Selects a key of a ConfigMap.<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b><a href="#inprocessconfigurationspecenvvarsindexvaluefromfieldref">fieldRef</a></b></td>
        <td>object</td>
        <td>
          Selects a field of the pod: supports metadata.name, metadata.namespace, `metadata.labels['&lt;KEY&gt;']`, `metadata.annotations['&lt;KEY&gt;']`,
spec.nodeName, spec.serviceAccountName, status.hostIP, status.podIP, status.podIPs.<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b><a href="#inprocessconfigurationspecenvvarsindexvaluefromresourcefieldref">resourceFieldRef</a></b></td>
        <td>object</td>
        <td>
          Selects a resource of the container: only resources limits and requests
(limits.cpu, limits.memory, limits.ephemeral-storage, requests.cpu, requests.memory and requests.ephemeral-storage) are currently supported.<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b><a href="#inprocessconfigurationspecenvvarsindexvaluefromsecretkeyref">secretKeyRef</a></b></td>
        <td>object</td>
        <td>
          Selects a key of a secret in the pod's namespace<br/>
        </td>
        <td>false</td>
      </tr></tbody>
</table>


### InProcessConfiguration.spec.envVars[index].valueFrom.configMapKeyRef
<sup><sup>[↩ Parent](#inprocessconfigurationspecenvvarsindexvaluefrom)</sup></sup>



Selects a key of a ConfigMap.

<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Description</th>
            <th>Required</th>
        </tr>
    </thead>
    <tbody><tr>
        <td><b>key</b></td>
        <td>string</td>
        <td>
          The key to select.<br/>
        </td>
        <td>true</td>
      </tr><tr>
        <td><b>name</b></td>
        <td>string</td>
        <td>
          Name of the referent.
This field is effectively required, but due to backwards compatibility is
allowed to be empty. Instances of this type with an empty value here are
almost certainly wrong.
More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names<br/>
          <br/>
            <i>Default</i>: <br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>optional</b></td>
        <td>boolean</td>
        <td>
          Specify whether the ConfigMap or its key must be defined<br/>
        </td>
        <td>false</td>
      </tr></tbody>
</table>


### InProcessConfiguration.spec.envVars[index].valueFrom.fieldRef
<sup><sup>[↩ Parent](#inprocessconfigurationspecenvvarsindexvaluefrom)</sup></sup>



Selects a field of the pod: supports metadata.name, metadata.namespace, `metadata.labels['&lt;KEY&gt;']`, `metadata.annotations['&lt;KEY&gt;']`,
spec.nodeName, spec.serviceAccountName, status.hostIP, status.podIP, status.podIPs.

<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Description</th>
            <th>Required</th>
        </tr>
    </thead>
    <tbody><tr>
        <td><b>fieldPath</b></td>
        <td>string</td>
        <td>
          Path of the field to select in the specified API version.<br/>
        </td>
        <td>true</td>
      </tr><tr>
        <td><b>apiVersion</b></td>
        <td>string</td>
        <td>
          Version of the schema the FieldPath is written in terms of, defaults to "v1".<br/>
        </td>
        <td>false</td>
      </tr></tbody>
</table>


### InProcessConfiguration.spec.envVars[index].valueFrom.resourceFieldRef
<sup><sup>[↩ Parent](#inprocessconfigurationspecenvvarsindexvaluefrom)</sup></sup>



Selects a resource of the container: only resources limits and requests
(limits.cpu, limits.memory, limits.ephemeral-storage, requests.cpu, requests.memory and requests.ephemeral-storage) are currently supported.

<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Description</th>
            <th>Required</th>
        </tr>
    </thead>
    <tbody><tr>
        <td><b>resource</b></td>
        <td>string</td>
        <td>
          Required: resource to select<br/>
        </td>
        <td>true</td>
      </tr><tr>
        <td><b>containerName</b></td>
        <td>string</td>
        <td>
          Container name: required for volumes, optional for env vars<br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>divisor</b></td>
        <td>int or string</td>
        <td>
          Specifies the output format of the exposed resources, defaults to "1"<br/>
        </td>
        <td>false</td>
      </tr></tbody>
</table>


### InProcessConfiguration.spec.envVars[index].valueFrom.secretKeyRef
<sup><sup>[↩ Parent](#inprocessconfigurationspecenvvarsindexvaluefrom)</sup></sup>



Selects a key of a secret in the pod's namespace

<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Description</th>
            <th>Required</th>
        </tr>
    </thead>
    <tbody><tr>
        <td><b>key</b></td>
        <td>string</td>
        <td>
          The key of the secret to select from.  Must be a valid secret key.<br/>
        </td>
        <td>true</td>
      </tr><tr>
        <td><b>name</b></td>
        <td>string</td>
        <td>
          Name of the referent.
This field is effectively required, but due to backwards compatibility is
allowed to be empty. Instances of this type with an empty value here are
almost certainly wrong.
More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names<br/>
          <br/>
            <i>Default</i>: <br/>
        </td>
        <td>false</td>
      </tr><tr>
        <td><b>optional</b></td>
        <td>boolean</td>
        <td>
          Specify whether the Secret or its key must be defined<br/>
        </td>
        <td>false</td>
      </tr></tbody>
</table>