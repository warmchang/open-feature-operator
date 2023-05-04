# Changelog

## [0.2.35](https://github.com/warmchang/open-feature-operator/compare/v0.2.34...v0.2.35) (2023-05-04)


### 🔄 Refactoring

* logging cleanup ([#308](https://github.com/warmchang/open-feature-operator/issues/308)) ([75bdd8b](https://github.com/warmchang/open-feature-operator/commit/75bdd8ba6292e432e0ed422398c69387d44f8ce6))
* update file mount path to conform with schema store regex ([#331](https://github.com/warmchang/open-feature-operator/issues/331)) ([56ea082](https://github.com/warmchang/open-feature-operator/commit/56ea082c99cf1f4ef1552ac79e3f5f5d2a883221))


### ✨ New Features

* add ff shortname, commit httpSyncConfiguration ([11e4652](https://github.com/warmchang/open-feature-operator/commit/11e46528fcd06cdc0c8e6f46944656224cd97441))
* add log format configuration options through helm chart ([#346](https://github.com/warmchang/open-feature-operator/issues/346)) ([bcef736](https://github.com/warmchang/open-feature-operator/commit/bcef7368fc4905b351f81f5dfa10eb4c26bf8764))
* backfill flagd-kubernetes-sync cluster role binding on startup ([#299](https://github.com/warmchang/open-feature-operator/issues/299)) ([02ca541](https://github.com/warmchang/open-feature-operator/commit/02ca541353afdbfe4cdc41f32f9399826d4f6fc5))
* default sync provider configuration ([#320](https://github.com/warmchang/open-feature-operator/issues/320)) ([7cba7e1](https://github.com/warmchang/open-feature-operator/commit/7cba7e14c223a083f02ff8313b899583253120f3))
* enable flagd probes ([#390](https://github.com/warmchang/open-feature-operator/issues/390)) ([41efb15](https://github.com/warmchang/open-feature-operator/commit/41efb155994b3cfb768cc39e59bfc09781c57f2e))
* flagd proxy resource ownership ([#442](https://github.com/warmchang/open-feature-operator/issues/442)) ([31b5f7b](https://github.com/warmchang/open-feature-operator/commit/31b5f7bdc62fde593c10797d0f177446aba5d71e))
* Helm configuration ([#304](https://github.com/warmchang/open-feature-operator/issues/304)) ([99edfeb](https://github.com/warmchang/open-feature-operator/commit/99edfeb8c32ada435f830c6799540ebdf3b5fcdd))
* improve deployment pattern ([#344](https://github.com/warmchang/open-feature-operator/issues/344)) ([572ba96](https://github.com/warmchang/open-feature-operator/commit/572ba961912ada2c07eb6143925d16ab6a6a85a3))
* introduce configurable resource limits for flagd sidecar ([e4affcf](https://github.com/warmchang/open-feature-operator/commit/e4affcfb0ccf13dc0406ef1c21c2b884a836f71f))
* introduce debugLogging parameter to FlagSourceConfiguration CRD ([#434](https://github.com/warmchang/open-feature-operator/issues/434)) ([26ae125](https://github.com/warmchang/open-feature-operator/commit/26ae1257f7611ea78dc34247b2f866b0d2043525))
* Introduced context to the readyz endpoint, added wait to test suite ([#336](https://github.com/warmchang/open-feature-operator/issues/336)) ([ed81c02](https://github.com/warmchang/open-feature-operator/commit/ed81c0284f8d759eb228d3af7030efb0b94ee280))
* introduced v1beta1 of featureflagconfiguration CRD with conversion webhook to v1alpha1 ([a45bdef](https://github.com/warmchang/open-feature-operator/commit/a45bdef5eec87738ce731af5825daffeb69eb6cb))
* kube-flagd-proxy deployment ([#412](https://github.com/warmchang/open-feature-operator/issues/412)) ([651c63c](https://github.com/warmchang/open-feature-operator/commit/651c63c5feeb00349db3233554ece2d289e9ccf2))
* migrate flagd startup argument to sources flag ([#427](https://github.com/warmchang/open-feature-operator/issues/427)) ([1c67f34](https://github.com/warmchang/open-feature-operator/commit/1c67f34dca6a6f58e09a7e8b56ce2a2523c1d260))
* structured the featureflagconfiguration CRD ([b056c7c](https://github.com/warmchang/open-feature-operator/commit/b056c7cdd76f4653c1a728342687beaa8279e314))
* **test:** substitute kuttl to bash e2e test ([#411](https://github.com/warmchang/open-feature-operator/issues/411)) ([ff199f1](https://github.com/warmchang/open-feature-operator/commit/ff199f1ae3c72d5472937eef7c2409b186bbb314))
* upgrade flagd to v0.3.0 ([20571e1](https://github.com/warmchang/open-feature-operator/commit/20571e1018e102ffbcf01b2518fcbf8b66a287be))


### 📚 Documentation

* add AND operator to sequential commands ([#368](https://github.com/warmchang/open-feature-operator/issues/368)) ([6f73a62](https://github.com/warmchang/open-feature-operator/commit/6f73a6214d87771f9555469fe4d60dbb6d301198))
* add killercoda demo link ([#413](https://github.com/warmchang/open-feature-operator/issues/413)) ([bbeeea2](https://github.com/warmchang/open-feature-operator/commit/bbeeea27feb3bca805a8be504c6ad447a580582d))
* automated demo deployment ([#310](https://github.com/warmchang/open-feature-operator/issues/310)) ([e9cb659](https://github.com/warmchang/open-feature-operator/commit/e9cb6598fadc440ed300231dbacf88926945724a))
* Doc fixes ([#469](https://github.com/warmchang/open-feature-operator/issues/469)) ([5a7918a](https://github.com/warmchang/open-feature-operator/commit/5a7918a94615621b6c6430e7ddec28c3d39a45e1))
* fix link to artifact hub ([9e9590b](https://github.com/warmchang/open-feature-operator/commit/9e9590b1d60b87b96a90f69ae89401362cc23d9b))
* fix rendering issue with operator resource config table ([#401](https://github.com/warmchang/open-feature-operator/issues/401)) ([71ea8a6](https://github.com/warmchang/open-feature-operator/commit/71ea8a68bbb97052822552ffce3c498c3da0e52d))
* improve getting started guide ([#288](https://github.com/warmchang/open-feature-operator/issues/288)) ([a5a009b](https://github.com/warmchang/open-feature-operator/commit/a5a009b8ea10dabf4c2034c54b1eb1e8d71e7c23))
* replace `make deploy-demo` command with a link to the `cloud-native-demo` repo ([#476](https://github.com/warmchang/open-feature-operator/issues/476)) ([fff12a8](https://github.com/warmchang/open-feature-operator/commit/fff12a8dca900478c8f58762ce00ebaf23958dc6))
* Update permissions docs ([#350](https://github.com/warmchang/open-feature-operator/issues/350)) ([e89ea75](https://github.com/warmchang/open-feature-operator/commit/e89ea7528d1e7546b2b4c0a81a105dda309f52b3))


### 🐛 Bug Fixes

* add sbom to ouput name ([#182](https://github.com/warmchang/open-feature-operator/issues/182)) ([5e939a8](https://github.com/warmchang/open-feature-operator/commit/5e939a8f67fbd095c18a6a2172bb856fe61dd173))
* artifact name and output file ([#187](https://github.com/warmchang/open-feature-operator/issues/187)) ([4dee157](https://github.com/warmchang/open-feature-operator/commit/4dee157d44c20fc925f9e33dbaae16c18f3d9b48))
* **deps:** update github.com/open-feature/schemas digest to 302d0fa ([#246](https://github.com/warmchang/open-feature-operator/issues/246)) ([7d22374](https://github.com/warmchang/open-feature-operator/commit/7d22374afb7a5e2e166550544d327ec7b5b3d1bf))
* **deps:** update github.com/open-feature/schemas digest to d638ecf ([a984836](https://github.com/warmchang/open-feature-operator/commit/a98483696f467270783858046132f02b3d338ac2))
* **deps:** update kubernetes packages to v0.25.3 ([8d6103d](https://github.com/warmchang/open-feature-operator/commit/8d6103d8d41e9fc6f3854ef6a27293a754160ff5))
* **deps:** update kubernetes packages to v0.25.4 ([75bab2d](https://github.com/warmchang/open-feature-operator/commit/75bab2d441c945d51f17f0d32195a217072c3c15))
* **deps:** update kubernetes packages to v0.26.3 ([#273](https://github.com/warmchang/open-feature-operator/issues/273)) ([abe56e1](https://github.com/warmchang/open-feature-operator/commit/abe56e14305309d4a4c776f4dfa3c8110cd16d23))
* **deps:** update module github.com/go-logr/logr to v1.2.4 ([#428](https://github.com/warmchang/open-feature-operator/issues/428)) ([8d07dab](https://github.com/warmchang/open-feature-operator/commit/8d07dab7eec3f467c84f09512bbf4c4cb066e35f))
* **deps:** update module github.com/onsi/gomega to v1.27.5 ([#357](https://github.com/warmchang/open-feature-operator/issues/357)) ([8624958](https://github.com/warmchang/open-feature-operator/commit/86249582d4bea32f9942c3940590ef399648e6e9))
* **deps:** update module github.com/onsi/gomega to v1.27.6 ([#429](https://github.com/warmchang/open-feature-operator/issues/429)) ([987815c](https://github.com/warmchang/open-feature-operator/commit/987815c05e933d3bfa4020a3864e4493b3b6e80d))
* **deps:** update module github.com/open-feature/schemas to v0.2.8 ([#269](https://github.com/warmchang/open-feature-operator/issues/269)) ([ed48060](https://github.com/warmchang/open-feature-operator/commit/ed48060b1f9e591ddadca4f9478728a823e10685))
* **deps:** update module github.com/stretchr/testify to v1.8.2 ([#396](https://github.com/warmchang/open-feature-operator/issues/396)) ([f24b6c4](https://github.com/warmchang/open-feature-operator/commit/f24b6c4e536f56cde412827606eacd722637da89))
* **deps:** update module go.uber.org/zap to v1.24.0 ([#268](https://github.com/warmchang/open-feature-operator/issues/268)) ([b7bdde8](https://github.com/warmchang/open-feature-operator/commit/b7bdde8944446621751e6ef70e6b0f0646adee21))
* **deps:** update module sigs.k8s.io/controller-runtime to v0.13.1 ([edeffcd](https://github.com/warmchang/open-feature-operator/commit/edeffcd3ef6fe9a8d52d0d5c414512ef8cd80629))
* **deps:** update module sigs.k8s.io/controller-runtime to v0.14.5 ([#279](https://github.com/warmchang/open-feature-operator/issues/279)) ([8a80bff](https://github.com/warmchang/open-feature-operator/commit/8a80bff886af404e897e6a247cea2f4c88d88499))
* **deps:** update module sigs.k8s.io/controller-runtime to v0.14.6 ([#426](https://github.com/warmchang/open-feature-operator/issues/426)) ([0e779e8](https://github.com/warmchang/open-feature-operator/commit/0e779e8d8f53861b0c1a824701ff8668b9fb1907))
* for helm issues ([#206](https://github.com/warmchang/open-feature-operator/issues/206)) ([39febd7](https://github.com/warmchang/open-feature-operator/commit/39febd76d1b996afdbc24399bcd08b502621c6cc))
* gave configmaps volume mounts a subpath to allow for multiple mounts ([#321](https://github.com/warmchang/open-feature-operator/issues/321)) ([2ec454c](https://github.com/warmchang/open-feature-operator/commit/2ec454c036149ebeaf34f81cbf4ad7895f0bb995))
* include release tag in helm charts publishing ([2746716](https://github.com/warmchang/open-feature-operator/commit/27467164dcd05b0220e0857bf79e42d62e7a40a9))
* mount dirs not files ([#326](https://github.com/warmchang/open-feature-operator/issues/326)) ([089ab3c](https://github.com/warmchang/open-feature-operator/commit/089ab3c48c0937e64060057e43ff07cf8fd47f67))
* nil pointer dereference ([#216](https://github.com/warmchang/open-feature-operator/issues/216)) ([d975066](https://github.com/warmchang/open-feature-operator/commit/d975066f96a5f9caf8af8d513076480a33943257))
* remove 'grpc://' prefix from proxy sync address ([#479](https://github.com/warmchang/open-feature-operator/issues/479)) ([50151ff](https://github.com/warmchang/open-feature-operator/commit/50151ffcfd239764da19e76cf657cd511ec882b0))
* remove redundant name ([#189](https://github.com/warmchang/open-feature-operator/issues/189)) ([664bd73](https://github.com/warmchang/open-feature-operator/commit/664bd7314e376b23a01247b5c027c04a9ac26329))
* remove unneeded OF namespace prefix from clusterrolebindings ([#453](https://github.com/warmchang/open-feature-operator/issues/453)) ([b23edef](https://github.com/warmchang/open-feature-operator/commit/b23edefc0d403e02dc2279bf275406bd988294f8))
* removed duplicate config map generation, resolve permissions issue ([#305](https://github.com/warmchang/open-feature-operator/issues/305)) ([eec16af](https://github.com/warmchang/open-feature-operator/commit/eec16af28eb963a3d0f276d382e808079e663a50))
* removed old prefix from flagd-proxy provider config ([#463](https://github.com/warmchang/open-feature-operator/issues/463)) ([39a99c6](https://github.com/warmchang/open-feature-operator/commit/39a99c622bb0a7a0fca63d07cc546b2a86f952a5))
* resolve issue with templated DNS name in cert ([65068df](https://github.com/warmchang/open-feature-operator/commit/65068df3019312a965271e50c52bbb90b68665c0))
* restrict permissions to only access specific CRB ([#436](https://github.com/warmchang/open-feature-operator/issues/436)) ([6f1f93c](https://github.com/warmchang/open-feature-operator/commit/6f1f93c98c7b8fbee534cc7db63fc396fa5b73c7))
* Security issues ([#348](https://github.com/warmchang/open-feature-operator/issues/348)) ([5bd0b19](https://github.com/warmchang/open-feature-operator/commit/5bd0b192a5db7f1557e1161e4bb425bbf0e31e2a))
* set defaultTag to INPUT_FLAGD_VERSION ([#332](https://github.com/warmchang/open-feature-operator/issues/332)) ([23547a1](https://github.com/warmchang/open-feature-operator/commit/23547a1e155e0cde2f085882bfd43128681466cd))
* set sbom dir ([#178](https://github.com/warmchang/open-feature-operator/issues/178)) ([143adf9](https://github.com/warmchang/open-feature-operator/commit/143adf910fe15a8b8af31dff48743352ab203d83))
* set sbom dir ([#180](https://github.com/warmchang/open-feature-operator/issues/180)) ([616272d](https://github.com/warmchang/open-feature-operator/commit/616272d6d693115a22839cf52eb8fd448609ad6c))
* uniqueness of featureflagconfiguration file path ([#323](https://github.com/warmchang/open-feature-operator/issues/323)) ([2b10945](https://github.com/warmchang/open-feature-operator/commit/2b109452893abd053640ffbb9c79b834b78feb7b))
* update flagd proxy env var prefix ([#440](https://github.com/warmchang/open-feature-operator/issues/440)) ([b451d47](https://github.com/warmchang/open-feature-operator/commit/b451d47184c37a5c218ce66a37a448f357dce11f))
* update flagd version ([#402](https://github.com/warmchang/open-feature-operator/issues/402)) ([dc6aa3c](https://github.com/warmchang/open-feature-operator/commit/dc6aa3c3dd9fec6c508b34608384247b63b42eeb))
* update x/net for CVE-2022-41721 ([#301](https://github.com/warmchang/open-feature-operator/issues/301)) ([bbe9837](https://github.com/warmchang/open-feature-operator/commit/bbe983786ff74b59046b95082d79f71089fe2b67))
* Version fix ([#284](https://github.com/warmchang/open-feature-operator/issues/284)) ([a9c6f15](https://github.com/warmchang/open-feature-operator/commit/a9c6f154589f1e00e60883c229b3ee29d7d2e9aa))


### 🧹 Chore

* adapt Makefile for local dev deployment + introduce report logs for e2e-tests ([#359](https://github.com/warmchang/open-feature-operator/issues/359)) ([17ac016](https://github.com/warmchang/open-feature-operator/commit/17ac016a3f326c726662c55dd19daed8777c76a1))
* add additional Kubernetes files ([#258](https://github.com/warmchang/open-feature-operator/issues/258)) ([b04928b](https://github.com/warmchang/open-feature-operator/commit/b04928b5d96196f6590f46e37a413d74d3186780))
* add additional sections to the release notes ([4bec5af](https://github.com/warmchang/open-feature-operator/commit/4bec5af5fc5fc589d920f0c17a1213a036b558a0))
* add all resources individually to tarball ([#345](https://github.com/warmchang/open-feature-operator/issues/345)) ([a0993dc](https://github.com/warmchang/open-feature-operator/commit/a0993dc5a2e1f3550aab2656b9ddeb08674dc896))
* add artifact hub metadata ([#372](https://github.com/warmchang/open-feature-operator/issues/372)) ([c6f539f](https://github.com/warmchang/open-feature-operator/commit/c6f539f5bdd9dc18ac197eb3303d91131e863011))
* add unit tests to pod webhook ([#419](https://github.com/warmchang/open-feature-operator/issues/419)) ([4290978](https://github.com/warmchang/open-feature-operator/commit/42909784b6a3a0642f07b5c5e093f9d4c549a21c))
* added cert-manager installation command to helm charts installation section ([2d4837d](https://github.com/warmchang/open-feature-operator/commit/2d4837d7e237f52962e5f025ca394ce1ea48658d))
* added crd configuration reconciliation e2e test ([f4a1c25](https://github.com/warmchang/open-feature-operator/commit/f4a1c256312026cb0fc7d5986d2e0ccddbf83ee9))
* attempt renovate fix ([48b6c7f](https://github.com/warmchang/open-feature-operator/commit/48b6c7fabce54270b06f53c033801be5ec100633))
* attempt versioning fix in test ([58d0145](https://github.com/warmchang/open-feature-operator/commit/58d0145f0a3ae1d67be002961faf82d8ef050015))
* automate release of charts ([552d345](https://github.com/warmchang/open-feature-operator/commit/552d34550c83ebaa06174c1c0ee34c0cdc1dd747))
* bump ENVTEST_K8S_VERSION to 1.25 ([#214](https://github.com/warmchang/open-feature-operator/issues/214)) ([a3d0609](https://github.com/warmchang/open-feature-operator/commit/a3d06090544310519e8574ca81873840082b6acf))
* bump go version in release-assets workflow ([#230](https://github.com/warmchang/open-feature-operator/issues/230)) ([8d4d587](https://github.com/warmchang/open-feature-operator/commit/8d4d58768fe194c5c99010ca9ee697ef9ebc84ae))
* **deps:** update actions/checkout action to v3 ([b56db1b](https://github.com/warmchang/open-feature-operator/commit/b56db1b7c03555bff76e1f0f96bbd6e427179e4a))
* **deps:** update actions/setup-go action to v4 ([#398](https://github.com/warmchang/open-feature-operator/issues/398)) ([ee9ecb9](https://github.com/warmchang/open-feature-operator/commit/ee9ecb9d693cdccbcac38a5c6c97d20a8a9c769f))
* **deps:** update amannn/action-semantic-pull-request action to v5 ([295dc91](https://github.com/warmchang/open-feature-operator/commit/295dc9157ff8345cbdd8f0d0d1e078c26af232f4))
* **deps:** update curlimages/curl docker tag to v7.88.1 ([#459](https://github.com/warmchang/open-feature-operator/issues/459)) ([ea98e1e](https://github.com/warmchang/open-feature-operator/commit/ea98e1e77ac616acc4aebf1ea042fc812486ece7))
* **deps:** update curlimages/curl docker tag to v8 ([#461](https://github.com/warmchang/open-feature-operator/issues/461)) ([1271eab](https://github.com/warmchang/open-feature-operator/commit/1271eab2eb4ad6aaab226116cd317345c02f55ac))
* **deps:** update dependency open-feature/flagd to v0.2.1 ([#462](https://github.com/warmchang/open-feature-operator/issues/462)) ([d2d53b7](https://github.com/warmchang/open-feature-operator/commit/d2d53b75791eef407ba0b1dd5377aff8277301ea))
* **deps:** update dependency open-feature/flagd to v0.3.1 ([#296](https://github.com/warmchang/open-feature-operator/issues/296)) ([1eff914](https://github.com/warmchang/open-feature-operator/commit/1eff914228d5ca04b9781db1e0ead1dd7aef0462))
* **deps:** update dependency open-feature/flagd to v0.3.2 ([#314](https://github.com/warmchang/open-feature-operator/issues/314)) ([dbfea97](https://github.com/warmchang/open-feature-operator/commit/dbfea97ac471faee34e168552dae2be6d2416b9c))
* **deps:** update dependency open-feature/flagd to v0.3.4 ([#327](https://github.com/warmchang/open-feature-operator/issues/327)) ([eb4d6ee](https://github.com/warmchang/open-feature-operator/commit/eb4d6ee4e7d8a29f8eb25fc649a93373eab4aca7))
* **deps:** update dependency open-feature/flagd to v0.4.0 ([#342](https://github.com/warmchang/open-feature-operator/issues/342)) ([0640f46](https://github.com/warmchang/open-feature-operator/commit/0640f469daa3c0adce920bb73e901fe83bc275e7))
* **deps:** update dependency open-feature/flagd to v0.4.1 ([#373](https://github.com/warmchang/open-feature-operator/issues/373)) ([756cf7a](https://github.com/warmchang/open-feature-operator/commit/756cf7a96c05fdfa8ffa2bf933225b84af400e37))
* **deps:** update dependency open-feature/flagd to v0.4.4 ([#400](https://github.com/warmchang/open-feature-operator/issues/400)) ([3e0a666](https://github.com/warmchang/open-feature-operator/commit/3e0a666f2824071c49250a4467d62b96a5af5ee7))
* **deps:** update docker/build-push-action action to v3 ([214bf57](https://github.com/warmchang/open-feature-operator/commit/214bf57f89de6e377d17d5f8f6c801fdfb2d7061))
* **deps:** update docker/build-push-action action to v4 ([#335](https://github.com/warmchang/open-feature-operator/issues/335)) ([a4cfad8](https://github.com/warmchang/open-feature-operator/commit/a4cfad87193c624fbc9cab5235fbea0adefdbb90))
* **deps:** update docker/login-action digest to 219c305 ([#365](https://github.com/warmchang/open-feature-operator/issues/365)) ([ee84954](https://github.com/warmchang/open-feature-operator/commit/ee849546322516019ea19a205c22c4ee38ac36ed))
* **deps:** update docker/login-action digest to 3da7dc6 ([#266](https://github.com/warmchang/open-feature-operator/issues/266)) ([7e8ed83](https://github.com/warmchang/open-feature-operator/commit/7e8ed830825b78cc9053ade134da979e44eb243d))
* **deps:** update docker/login-action digest to 65b78e6 ([#421](https://github.com/warmchang/open-feature-operator/issues/421)) ([8d2ebe2](https://github.com/warmchang/open-feature-operator/commit/8d2ebe27193379fb54e5a39455e8db787f8eae89))
* **deps:** update docker/login-action digest to f4ef78c ([71b37aa](https://github.com/warmchang/open-feature-operator/commit/71b37aa5e5928234bf403afa123b3665f64c294c))
* **deps:** update docker/metadata-action digest to 3f6690a ([#432](https://github.com/warmchang/open-feature-operator/issues/432)) ([991b2bd](https://github.com/warmchang/open-feature-operator/commit/991b2bd3c320b8b576812f72a2d98ab30436f6c8))
* **deps:** update docker/metadata-action digest to 5739616 ([7b82bd0](https://github.com/warmchang/open-feature-operator/commit/7b82bd0a2a2c1119029c97d930f3b6606de2059b))
* **deps:** update docker/metadata-action digest to 766400c ([#267](https://github.com/warmchang/open-feature-operator/issues/267)) ([38a1464](https://github.com/warmchang/open-feature-operator/commit/38a14644e687b928e51d1350f6d57ef9d493330c))
* **deps:** update docker/metadata-action digest to 9ec57ed ([#366](https://github.com/warmchang/open-feature-operator/issues/366)) ([884d444](https://github.com/warmchang/open-feature-operator/commit/884d44422ad7bfa28a8fb88156cd66e252e2eba5))
* **deps:** update gcr.io/kubebuilder/kube-rbac-proxy docker tag to v0.13.0 ([86953f6](https://github.com/warmchang/open-feature-operator/commit/86953f63c691cd4cce56854de46022a7e898f82c))
* **deps:** update gcr.io/kubebuilder/kube-rbac-proxy docker tag to v0.13.1 ([2462b1c](https://github.com/warmchang/open-feature-operator/commit/2462b1c2b298927bea0d43eb03ee885e6d43c4c9))
* **deps:** update gcr.io/kubebuilder/kube-rbac-proxy docker tag to v0.13.1 ([31570b2](https://github.com/warmchang/open-feature-operator/commit/31570b2041ab143d6e1e6cdce90f03c449b03e17))
* **deps:** update gcr.io/kubebuilder/kube-rbac-proxy docker tag to v0.14.0 ([#376](https://github.com/warmchang/open-feature-operator/issues/376)) ([708e4bc](https://github.com/warmchang/open-feature-operator/commit/708e4bc44d8493d4f0aaa7f7036c2b7ecd2efd32))
* **deps:** update ghcr.io/open-feature/flagd docker tag to v0.3.2 ([#315](https://github.com/warmchang/open-feature-operator/issues/315)) ([c178c49](https://github.com/warmchang/open-feature-operator/commit/c178c49f585e6e8ff28d8dff49c6c95930dd4cef))
* **deps:** update ghcr.io/open-feature/flagd docker tag to v0.3.4 ([#328](https://github.com/warmchang/open-feature-operator/issues/328)) ([f96246f](https://github.com/warmchang/open-feature-operator/commit/f96246f748b00094bfb82b6b0dcf035a17128dc9))
* **deps:** update ghcr.io/open-feature/flagd docker tag to v0.4.4 ([#381](https://github.com/warmchang/open-feature-operator/issues/381)) ([a253761](https://github.com/warmchang/open-feature-operator/commit/a253761af8565fdcf6e6f9ca92c740f25b4b0620))
* **deps:** update ghcr.io/open-feature/open-feature-operator docker tag to v0.2.16 ([7644166](https://github.com/warmchang/open-feature-operator/commit/764416681b6516ab07bda146afa1d3e4ac142dba))
* **deps:** update golang docker tag to v1.20.2 ([#374](https://github.com/warmchang/open-feature-operator/issues/374)) ([e2de529](https://github.com/warmchang/open-feature-operator/commit/e2de52997b44835a4a8515e9fd37c976d3539272))
* **deps:** update golang docker tag to v1.20.3 ([#445](https://github.com/warmchang/open-feature-operator/issues/445)) ([b8f6c5b](https://github.com/warmchang/open-feature-operator/commit/b8f6c5b9e7bfc986f2208b2d7a2f402d7210ca7a))
* **deps:** update helm/kind-action action to v1.5.0 ([#277](https://github.com/warmchang/open-feature-operator/issues/277)) ([15ad251](https://github.com/warmchang/open-feature-operator/commit/15ad251614020a4581de015ffc5c721101326ead))
* **deps:** update module golang.org/x/net to v0.8.0 ([#397](https://github.com/warmchang/open-feature-operator/issues/397)) ([096c889](https://github.com/warmchang/open-feature-operator/commit/096c889c87e80b5cfef0254869dc1e096ee23ad8))
* **deps:** update module golang.org/x/net to v0.9.0 ([#451](https://github.com/warmchang/open-feature-operator/issues/451)) ([4cbe4f1](https://github.com/warmchang/open-feature-operator/commit/4cbe4f1a02517d89a53fde6ca1a5861da2691747))
* **deps:** update open-feature/flagd ([#457](https://github.com/warmchang/open-feature-operator/issues/457)) ([db9af7a](https://github.com/warmchang/open-feature-operator/commit/db9af7a02dbfcd4be10b170dab4bb5e65614221f))
* **deps:** update open-feature/flagd ([#466](https://github.com/warmchang/open-feature-operator/issues/466)) ([3b8d156](https://github.com/warmchang/open-feature-operator/commit/3b8d1564af5fa2991f3e26a0cb8fbf6ff722a9b1))
* **deps:** update open-feature/flagd to v0.5.0 ([#422](https://github.com/warmchang/open-feature-operator/issues/422)) ([6846aa2](https://github.com/warmchang/open-feature-operator/commit/6846aa206a9ffb4aa9b1cff1ca7078b93ede927c))
* **docs:** add concepts doc, add filepath docs ([#340](https://github.com/warmchang/open-feature-operator/issues/340)) ([5f83920](https://github.com/warmchang/open-feature-operator/commit/5f839209008ced69198cdf909659c0001e1b3910))
* document crd upgrades ([#361](https://github.com/warmchang/open-feature-operator/issues/361)) ([e708990](https://github.com/warmchang/open-feature-operator/commit/e70899081b8c0864c8ef17f75275d67b26b63c20))
* e2e test for openfeature.dev/enabled annotation set to false ([#375](https://github.com/warmchang/open-feature-operator/issues/375)) ([b03fb14](https://github.com/warmchang/open-feature-operator/commit/b03fb145e317f987727d76b98041fa783e5c2202))
* extract flagd container injection into its own component ([#474](https://github.com/warmchang/open-feature-operator/issues/474)) ([9ed8e59](https://github.com/warmchang/open-feature-operator/commit/9ed8e598f8612f5f0935dbd115cd7a8053aa1210))
* fix image name in helm chart ([f2782c6](https://github.com/warmchang/open-feature-operator/commit/f2782c6d381fee59b37f3be3f5b1399a1ee7eb29))
* fix make helm-package command in release charts workflow ([3fc9735](https://github.com/warmchang/open-feature-operator/commit/3fc9735148619771693bfbb2a92f62e12bfd9480))
* fix renovate config, add recommended preset ([#418](https://github.com/warmchang/open-feature-operator/issues/418)) ([78c5970](https://github.com/warmchang/open-feature-operator/commit/78c597024241158ebf2e9b07e82610766efd85de))
* gitignore generate charts ([#356](https://github.com/warmchang/open-feature-operator/issues/356)) ([250b5ab](https://github.com/warmchang/open-feature-operator/commit/250b5abd6d6dedebf23bdf931777e53ec116565f))
* go version bump ([5219a1e](https://github.com/warmchang/open-feature-operator/commit/5219a1e6a4d449bcdbae626f2a8cba5dab622426))
* how to implement a new crd version ([#227](https://github.com/warmchang/open-feature-operator/issues/227)) ([1b01cec](https://github.com/warmchang/open-feature-operator/commit/1b01cec8e81b1a6dd9da0f5a94871eafa934d2a9))
* improve container build layer caching ([#414](https://github.com/warmchang/open-feature-operator/issues/414)) ([3212eba](https://github.com/warmchang/open-feature-operator/commit/3212eba809744c8dc1c94d8bf558523a0fbbf326))
* improve formatting and content ([#384](https://github.com/warmchang/open-feature-operator/issues/384)) ([c5a6a32](https://github.com/warmchang/open-feature-operator/commit/c5a6a32f0ccccc6449fc581de08c283434c1adb6))
* increase backoffLimit for inject-flagd ([#423](https://github.com/warmchang/open-feature-operator/issues/423)) ([29d7cf0](https://github.com/warmchang/open-feature-operator/commit/29d7cf069d68ce2b81718b0297194b3ba53c3ed9))
* integration tests for pod mutation webhook & featureflagconfiguration validation webhook ([2295659](https://github.com/warmchang/open-feature-operator/commit/2295659b47dfff46a0690b051db6a78c368b576c))
* introduce additional unit tests for api packages ([#420](https://github.com/warmchang/open-feature-operator/issues/420)) ([5ba5bc9](https://github.com/warmchang/open-feature-operator/commit/5ba5bc97faa8bf18a07a380d685c518f6e093145))
* **main:** release 0.2.11 ([#177](https://github.com/warmchang/open-feature-operator/issues/177)) ([8cd768e](https://github.com/warmchang/open-feature-operator/commit/8cd768e342266d766c7b85badcb015c76a4ed77a))
* **main:** release 0.2.12 ([#179](https://github.com/warmchang/open-feature-operator/issues/179)) ([fe3ca2d](https://github.com/warmchang/open-feature-operator/commit/fe3ca2d3e28a7044c8ff5ff1481ea20a3cd914e1))
* **main:** release 0.2.13 ([#181](https://github.com/warmchang/open-feature-operator/issues/181)) ([e685eae](https://github.com/warmchang/open-feature-operator/commit/e685eae3c84df53d890c9ab009c4f10e3ca14a36))
* **main:** release 0.2.14 ([#183](https://github.com/warmchang/open-feature-operator/issues/183)) ([0145eca](https://github.com/warmchang/open-feature-operator/commit/0145eca05faa525800a96db01c3e3833443eccf3))
* **main:** release 0.2.15 ([#188](https://github.com/warmchang/open-feature-operator/issues/188)) ([0068511](https://github.com/warmchang/open-feature-operator/commit/0068511e46b093dc7064c8026302feab7c2a3fbf))
* **main:** release 0.2.16 ([59af227](https://github.com/warmchang/open-feature-operator/commit/59af227f36586dff5d4d3943cefa7038ab7540a5))
* **main:** release 0.2.17 ([9546195](https://github.com/warmchang/open-feature-operator/commit/9546195d0d30f374780e72e59a39c01ac045d5c3))
* **main:** release 0.2.17 ([#208](https://github.com/warmchang/open-feature-operator/issues/208)) ([f375eb2](https://github.com/warmchang/open-feature-operator/commit/f375eb2232f588931c7391367d8cfb58f026eb89))
* **main:** release 0.2.18 ([#218](https://github.com/warmchang/open-feature-operator/issues/218)) ([d4be9ae](https://github.com/warmchang/open-feature-operator/commit/d4be9ae7280a7a5c0448a3efa23f59bf5d05096c))
* **main:** release 0.2.19 ([12b3934](https://github.com/warmchang/open-feature-operator/commit/12b3934ae20874ffe822036d4e0242bf95ce09c2))
* **main:** release 0.2.20 ([d22af86](https://github.com/warmchang/open-feature-operator/commit/d22af86e258a2ffa85c986a4898da9f6e27fb2e5))
* **main:** release 0.2.21 ([df8059f](https://github.com/warmchang/open-feature-operator/commit/df8059f183fda3aa063df8c6d054163c0dd3cfb1))
* **main:** release 0.2.22 ([#283](https://github.com/warmchang/open-feature-operator/issues/283)) ([40f5c0e](https://github.com/warmchang/open-feature-operator/commit/40f5c0e4135e19ba152285f43bd2627ea7c0be73))
* **main:** release 0.2.23 ([#290](https://github.com/warmchang/open-feature-operator/issues/290)) ([53ef2b9](https://github.com/warmchang/open-feature-operator/commit/53ef2b95a5b829ce30d10b9ae535842511169a5f))
* **main:** release 0.2.24 ([#300](https://github.com/warmchang/open-feature-operator/issues/300)) ([6a78925](https://github.com/warmchang/open-feature-operator/commit/6a78925e2fe852a02845acc32309784bb0dbf816))
* **main:** release 0.2.25 ([#306](https://github.com/warmchang/open-feature-operator/issues/306)) ([27f7d4d](https://github.com/warmchang/open-feature-operator/commit/27f7d4df57ad23da45eaeafc94a37b7f392f3c0e))
* **main:** release 0.2.26 ([#316](https://github.com/warmchang/open-feature-operator/issues/316)) ([d7e9559](https://github.com/warmchang/open-feature-operator/commit/d7e9559a9f60b2eab5a6e86fea734c04ad05980a))
* **main:** release 0.2.27 ([#322](https://github.com/warmchang/open-feature-operator/issues/322)) ([256894f](https://github.com/warmchang/open-feature-operator/commit/256894fe52797cef22b7186d354ec6056224883a))
* **main:** release 0.2.28 ([#330](https://github.com/warmchang/open-feature-operator/issues/330)) ([312e91e](https://github.com/warmchang/open-feature-operator/commit/312e91e6f9c1c44b9d642c74e031742f78c0f7f9))
* **main:** release 0.2.29 ([#339](https://github.com/warmchang/open-feature-operator/issues/339)) ([8b779b1](https://github.com/warmchang/open-feature-operator/commit/8b779b1855de171b0f81197d8850dbd2dff9322b))
* **main:** release 0.2.30 ([#363](https://github.com/warmchang/open-feature-operator/issues/363)) ([945aa6b](https://github.com/warmchang/open-feature-operator/commit/945aa6b81d27803a37771b90a08f5a7a79bb8085))
* **main:** release 0.2.31 ([#403](https://github.com/warmchang/open-feature-operator/issues/403)) ([42f9b00](https://github.com/warmchang/open-feature-operator/commit/42f9b007d391137b01bf9bc36bc40666d16c18b3))
* **main:** release 0.2.32 ([#407](https://github.com/warmchang/open-feature-operator/issues/407)) ([e0d639a](https://github.com/warmchang/open-feature-operator/commit/e0d639a4f4261f68bedf507fd492a8fff11c4dc2))
* **main:** release 0.2.33 ([#464](https://github.com/warmchang/open-feature-operator/issues/464)) ([11e671d](https://github.com/warmchang/open-feature-operator/commit/11e671d248c1b5e1b89a2be991540646c07a56e4))
* **main:** release 0.2.34 ([#467](https://github.com/warmchang/open-feature-operator/issues/467)) ([4fc60dc](https://github.com/warmchang/open-feature-operator/commit/4fc60dc49d8dbc16b402be333a157212145f6ab6))
* refactor admission webhook tests ([#409](https://github.com/warmchang/open-feature-operator/issues/409)) ([29c7c28](https://github.com/warmchang/open-feature-operator/commit/29c7c28b4a6fb76bc565e32f46d0ab74fc2e5371))
* refactor pod webhook mutator ([#410](https://github.com/warmchang/open-feature-operator/issues/410)) ([2a86b03](https://github.com/warmchang/open-feature-operator/commit/2a86b032888fef4bd3e7d93e3a5cb1cc376fcd22))
* refactored component test using fake client ([#435](https://github.com/warmchang/open-feature-operator/issues/435)) ([08a50ac](https://github.com/warmchang/open-feature-operator/commit/08a50accff516be1f8226c4f1051eef8843c9190))
* remove ignored renovate paths ([#441](https://github.com/warmchang/open-feature-operator/issues/441)) ([c1d8929](https://github.com/warmchang/open-feature-operator/commit/c1d89291d75ef0d594a071ef5055b55a404d9b73))
* remove namespace argument from e2e example in readme ([#217](https://github.com/warmchang/open-feature-operator/issues/217)) ([cb3b06d](https://github.com/warmchang/open-feature-operator/commit/cb3b06dd41c71de332faa93008a4425069dabdd2))
* remove pre alpha badges ([#317](https://github.com/warmchang/open-feature-operator/issues/317)) ([5fcf637](https://github.com/warmchang/open-feature-operator/commit/5fcf637dc6a1a18bb1234ec8a621195a8c71551e))
* remove published charts ([9dafe03](https://github.com/warmchang/open-feature-operator/commit/9dafe03a115fec6c1d2b998d0b6d98c00c5586cb))
* remove unneeded conversion webhooks + introduce unit tests for conversion functions ([#385](https://github.com/warmchang/open-feature-operator/issues/385)) ([dd34801](https://github.com/warmchang/open-feature-operator/commit/dd34801fd71ac4f1e6c0b0f39f78ddf738f5601d))
* renovate - force semantic commits ([152bf59](https://github.com/warmchang/open-feature-operator/commit/152bf59d4e5edf6ad6fa304f12093d12e0293491))
* renovate regex manager to monitor FLAGD_VERSION in Makefile ([e7f5e4b](https://github.com/warmchang/open-feature-operator/commit/e7f5e4b5eaf0107b01a04f71bb57791e1ba7a3ee))
* reorder containers in e2e assertion ([1d895c3](https://github.com/warmchang/open-feature-operator/commit/1d895c33c32cefc9858cf2ef0f283d1ba62a4f00))
* revert kustomization image name change ([#232](https://github.com/warmchang/open-feature-operator/issues/232)) ([0956a00](https://github.com/warmchang/open-feature-operator/commit/0956a0054003ba57c8bd890a3bdf4030a42a6607))
* run e2e test as a part of the github workflow ([99bb25c](https://github.com/warmchang/open-feature-operator/commit/99bb25cc134f3d967eea3fc5ea7ebc7c0467d99f))
* split controllers to separate packages + cover them with unit tests ([#404](https://github.com/warmchang/open-feature-operator/issues/404)) ([6ed4cef](https://github.com/warmchang/open-feature-operator/commit/6ed4cef4a7d1ec889300459f73e930d4b6d2ba6f))
* test filepath sync config change is reconciliated ([#338](https://github.com/warmchang/open-feature-operator/issues/338)) ([101729a](https://github.com/warmchang/open-feature-operator/commit/101729ad587d63541227c7eb9088ff67bf412640))
* test multiple sync providers ([#325](https://github.com/warmchang/open-feature-operator/issues/325)) ([f3fe057](https://github.com/warmchang/open-feature-operator/commit/f3fe057e180528944110a6841239d3f9d471086b))
* threat modeling ([#309](https://github.com/warmchang/open-feature-operator/issues/309)) ([dc7d935](https://github.com/warmchang/open-feature-operator/commit/dc7d9351b7f75bcc8e8eda3c3ea1d72e145955be))
* troubleshoot renovate ([de4ac14](https://github.com/warmchang/open-feature-operator/commit/de4ac1475717201ec6a828ffc7700d3c28de4d33))
* troubleshoot renovate ([89a7b5b](https://github.com/warmchang/open-feature-operator/commit/89a7b5b9890f127a5af1d321f40b8f2a8635fcb5))
* troubleshoot renovate ([244bd3a](https://github.com/warmchang/open-feature-operator/commit/244bd3ade508c476a9783c9ee11d608e2536bb9f))
* troubleshoot renovate ([eafa670](https://github.com/warmchang/open-feature-operator/commit/eafa6702e1663a02b24b48e3b61ea6252b2a9b40))
* troubleshoot renovate ([c3d9523](https://github.com/warmchang/open-feature-operator/commit/c3d95232d0f1ca6e8c898ffffb165537462fe2e9))
* troubleshoot renovatge ([35054cb](https://github.com/warmchang/open-feature-operator/commit/35054cb6917dcacbafb9fbccb00a85493922f245))
* troubleshoot renvoate ([7ac3c90](https://github.com/warmchang/open-feature-operator/commit/7ac3c90a358baf6f0dd00bd2f7295665ebf46a59))
* update build badge to new format ([13e85de](https://github.com/warmchang/open-feature-operator/commit/13e85de7764b602f8b08687272f6b6483b6d13f0))
* update charts to v0.2.18 ([d5fc087](https://github.com/warmchang/open-feature-operator/commit/d5fc08762dab469ecd4f62219d2e0333c507dd46))
* update charts to v0.2.19 ([fbd82eb](https://github.com/warmchang/open-feature-operator/commit/fbd82eb56ba322b161476cebbc881f2535b1527f))
* update CODEOWNERS ([edb1592](https://github.com/warmchang/open-feature-operator/commit/edb15923ff8b029f05553296df4bb135b8f697d2))
* update codeowners to use cloud native team ([6133060](https://github.com/warmchang/open-feature-operator/commit/613306011016a3cbb7fbc23a2273aecfd26a3bbf))
* update flagd renovate detection ([#439](https://github.com/warmchang/open-feature-operator/issues/439)) ([3d1540c](https://github.com/warmchang/open-feature-operator/commit/3d1540c67c7d43c69feb61654b7d2a3c8a72a5a1))
* update renovate config to watch the assert yaml directly ([9ef25a0](https://github.com/warmchang/open-feature-operator/commit/9ef25a0abbdeb15666679fd43d4f2c032b825722))
* upgrade ENVTEST_K8S_VERSION to 1.26.1 ([#360](https://github.com/warmchang/open-feature-operator/issues/360)) ([5e01c24](https://github.com/warmchang/open-feature-operator/commit/5e01c249a0da46eea0f964f2ded69a4e20c10335))
* use renovate to bump flagd version ([#395](https://github.com/warmchang/open-feature-operator/issues/395)) ([fd5b072](https://github.com/warmchang/open-feature-operator/commit/fd5b072214f1c3c74dfc4bc53ca1ff6c14d72ffa))

## [0.2.34](https://github.com/open-feature/open-feature-operator/compare/v0.2.33...v0.2.34) (2023-04-13)


### 🧹 Chore

* **deps:** update open-feature/flagd ([#466](https://github.com/open-feature/open-feature-operator/issues/466)) ([3b8d156](https://github.com/open-feature/open-feature-operator/commit/3b8d1564af5fa2991f3e26a0cb8fbf6ff722a9b1))

## [0.2.33](https://github.com/open-feature/open-feature-operator/compare/v0.2.32...v0.2.33) (2023-04-12)


### 🐛 Bug Fixes

* removed old prefix from flagd-proxy provider config ([#463](https://github.com/open-feature/open-feature-operator/issues/463)) ([39a99c6](https://github.com/open-feature/open-feature-operator/commit/39a99c622bb0a7a0fca63d07cc546b2a86f952a5))

## [0.2.32](https://github.com/open-feature/open-feature-operator/compare/v0.2.31...v0.2.32) (2023-04-12)


### 📚 Documentation

* add killercoda demo link ([#413](https://github.com/open-feature/open-feature-operator/issues/413)) ([bbeeea2](https://github.com/open-feature/open-feature-operator/commit/bbeeea27feb3bca805a8be504c6ad447a580582d))


### 🐛 Bug Fixes

* **deps:** update kubernetes packages to v0.26.3 ([#273](https://github.com/open-feature/open-feature-operator/issues/273)) ([abe56e1](https://github.com/open-feature/open-feature-operator/commit/abe56e14305309d4a4c776f4dfa3c8110cd16d23))
* **deps:** update module github.com/go-logr/logr to v1.2.4 ([#428](https://github.com/open-feature/open-feature-operator/issues/428)) ([8d07dab](https://github.com/open-feature/open-feature-operator/commit/8d07dab7eec3f467c84f09512bbf4c4cb066e35f))
* **deps:** update module github.com/onsi/gomega to v1.27.5 ([#357](https://github.com/open-feature/open-feature-operator/issues/357)) ([8624958](https://github.com/open-feature/open-feature-operator/commit/86249582d4bea32f9942c3940590ef399648e6e9))
* **deps:** update module github.com/onsi/gomega to v1.27.6 ([#429](https://github.com/open-feature/open-feature-operator/issues/429)) ([987815c](https://github.com/open-feature/open-feature-operator/commit/987815c05e933d3bfa4020a3864e4493b3b6e80d))
* **deps:** update module github.com/stretchr/testify to v1.8.2 ([#396](https://github.com/open-feature/open-feature-operator/issues/396)) ([f24b6c4](https://github.com/open-feature/open-feature-operator/commit/f24b6c4e536f56cde412827606eacd722637da89))
* **deps:** update module sigs.k8s.io/controller-runtime to v0.14.6 ([#426](https://github.com/open-feature/open-feature-operator/issues/426)) ([0e779e8](https://github.com/open-feature/open-feature-operator/commit/0e779e8d8f53861b0c1a824701ff8668b9fb1907))
* remove unneeded OF namespace prefix from clusterrolebindings ([#453](https://github.com/open-feature/open-feature-operator/issues/453)) ([b23edef](https://github.com/open-feature/open-feature-operator/commit/b23edefc0d403e02dc2279bf275406bd988294f8))
* restrict permissions to only access specific CRB ([#436](https://github.com/open-feature/open-feature-operator/issues/436)) ([6f1f93c](https://github.com/open-feature/open-feature-operator/commit/6f1f93c98c7b8fbee534cc7db63fc396fa5b73c7))
* update flagd proxy env var prefix ([#440](https://github.com/open-feature/open-feature-operator/issues/440)) ([b451d47](https://github.com/open-feature/open-feature-operator/commit/b451d47184c37a5c218ce66a37a448f357dce11f))


### ✨ New Features

* flagd proxy resource ownership ([#442](https://github.com/open-feature/open-feature-operator/issues/442)) ([31b5f7b](https://github.com/open-feature/open-feature-operator/commit/31b5f7bdc62fde593c10797d0f177446aba5d71e))
* introduce debugLogging parameter to FlagSourceConfiguration CRD ([#434](https://github.com/open-feature/open-feature-operator/issues/434)) ([26ae125](https://github.com/open-feature/open-feature-operator/commit/26ae1257f7611ea78dc34247b2f866b0d2043525))
* kube-flagd-proxy deployment ([#412](https://github.com/open-feature/open-feature-operator/issues/412)) ([651c63c](https://github.com/open-feature/open-feature-operator/commit/651c63c5feeb00349db3233554ece2d289e9ccf2))
* migrate flagd startup argument to sources flag ([#427](https://github.com/open-feature/open-feature-operator/issues/427)) ([1c67f34](https://github.com/open-feature/open-feature-operator/commit/1c67f34dca6a6f58e09a7e8b56ce2a2523c1d260))
* **test:** substitute kuttl to bash e2e test ([#411](https://github.com/open-feature/open-feature-operator/issues/411)) ([ff199f1](https://github.com/open-feature/open-feature-operator/commit/ff199f1ae3c72d5472937eef7c2409b186bbb314))


### 🧹 Chore

* add unit tests to pod webhook ([#419](https://github.com/open-feature/open-feature-operator/issues/419)) ([4290978](https://github.com/open-feature/open-feature-operator/commit/42909784b6a3a0642f07b5c5e093f9d4c549a21c))
* attempt renovate fix ([48b6c7f](https://github.com/open-feature/open-feature-operator/commit/48b6c7fabce54270b06f53c033801be5ec100633))
* attempt versioning fix in test ([58d0145](https://github.com/open-feature/open-feature-operator/commit/58d0145f0a3ae1d67be002961faf82d8ef050015))
* **deps:** update actions/setup-go action to v4 ([#398](https://github.com/open-feature/open-feature-operator/issues/398)) ([ee9ecb9](https://github.com/open-feature/open-feature-operator/commit/ee9ecb9d693cdccbcac38a5c6c97d20a8a9c769f))
* **deps:** update dependency open-feature/flagd to v0.2.1 ([#462](https://github.com/open-feature/open-feature-operator/issues/462)) ([d2d53b7](https://github.com/open-feature/open-feature-operator/commit/d2d53b75791eef407ba0b1dd5377aff8277301ea))
* **deps:** update docker/login-action digest to 65b78e6 ([#421](https://github.com/open-feature/open-feature-operator/issues/421)) ([8d2ebe2](https://github.com/open-feature/open-feature-operator/commit/8d2ebe27193379fb54e5a39455e8db787f8eae89))
* **deps:** update docker/metadata-action digest to 3f6690a ([#432](https://github.com/open-feature/open-feature-operator/issues/432)) ([991b2bd](https://github.com/open-feature/open-feature-operator/commit/991b2bd3c320b8b576812f72a2d98ab30436f6c8))
* **deps:** update golang docker tag to v1.20.3 ([#445](https://github.com/open-feature/open-feature-operator/issues/445)) ([b8f6c5b](https://github.com/open-feature/open-feature-operator/commit/b8f6c5b9e7bfc986f2208b2d7a2f402d7210ca7a))
* **deps:** update module golang.org/x/net to v0.8.0 ([#397](https://github.com/open-feature/open-feature-operator/issues/397)) ([096c889](https://github.com/open-feature/open-feature-operator/commit/096c889c87e80b5cfef0254869dc1e096ee23ad8))
* **deps:** update module golang.org/x/net to v0.9.0 ([#451](https://github.com/open-feature/open-feature-operator/issues/451)) ([4cbe4f1](https://github.com/open-feature/open-feature-operator/commit/4cbe4f1a02517d89a53fde6ca1a5861da2691747))
* **deps:** update open-feature/flagd ([#457](https://github.com/open-feature/open-feature-operator/issues/457)) ([db9af7a](https://github.com/open-feature/open-feature-operator/commit/db9af7a02dbfcd4be10b170dab4bb5e65614221f))
* **deps:** update open-feature/flagd to v0.5.0 ([#422](https://github.com/open-feature/open-feature-operator/issues/422)) ([6846aa2](https://github.com/open-feature/open-feature-operator/commit/6846aa206a9ffb4aa9b1cff1ca7078b93ede927c))
* fix renovate config, add recommended preset ([#418](https://github.com/open-feature/open-feature-operator/issues/418)) ([78c5970](https://github.com/open-feature/open-feature-operator/commit/78c597024241158ebf2e9b07e82610766efd85de))
* improve container build layer caching ([#414](https://github.com/open-feature/open-feature-operator/issues/414)) ([3212eba](https://github.com/open-feature/open-feature-operator/commit/3212eba809744c8dc1c94d8bf558523a0fbbf326))
* increase backoffLimit for inject-flagd ([#423](https://github.com/open-feature/open-feature-operator/issues/423)) ([29d7cf0](https://github.com/open-feature/open-feature-operator/commit/29d7cf069d68ce2b81718b0297194b3ba53c3ed9))
* introduce additional unit tests for api packages ([#420](https://github.com/open-feature/open-feature-operator/issues/420)) ([5ba5bc9](https://github.com/open-feature/open-feature-operator/commit/5ba5bc97faa8bf18a07a380d685c518f6e093145))
* refactor admission webhook tests ([#409](https://github.com/open-feature/open-feature-operator/issues/409)) ([29c7c28](https://github.com/open-feature/open-feature-operator/commit/29c7c28b4a6fb76bc565e32f46d0ab74fc2e5371))
* refactor pod webhook mutator ([#410](https://github.com/open-feature/open-feature-operator/issues/410)) ([2a86b03](https://github.com/open-feature/open-feature-operator/commit/2a86b032888fef4bd3e7d93e3a5cb1cc376fcd22))
* refactored component test using fake client ([#435](https://github.com/open-feature/open-feature-operator/issues/435)) ([08a50ac](https://github.com/open-feature/open-feature-operator/commit/08a50accff516be1f8226c4f1051eef8843c9190))
* remove ignored renovate paths ([#441](https://github.com/open-feature/open-feature-operator/issues/441)) ([c1d8929](https://github.com/open-feature/open-feature-operator/commit/c1d89291d75ef0d594a071ef5055b55a404d9b73))
* reorder containers in e2e assertion ([1d895c3](https://github.com/open-feature/open-feature-operator/commit/1d895c33c32cefc9858cf2ef0f283d1ba62a4f00))
* split controllers to separate packages + cover them with unit tests ([#404](https://github.com/open-feature/open-feature-operator/issues/404)) ([6ed4cef](https://github.com/open-feature/open-feature-operator/commit/6ed4cef4a7d1ec889300459f73e930d4b6d2ba6f))
* troubleshoot renovate ([de4ac14](https://github.com/open-feature/open-feature-operator/commit/de4ac1475717201ec6a828ffc7700d3c28de4d33))
* troubleshoot renovate ([89a7b5b](https://github.com/open-feature/open-feature-operator/commit/89a7b5b9890f127a5af1d321f40b8f2a8635fcb5))
* troubleshoot renovate ([244bd3a](https://github.com/open-feature/open-feature-operator/commit/244bd3ade508c476a9783c9ee11d608e2536bb9f))
* troubleshoot renovate ([eafa670](https://github.com/open-feature/open-feature-operator/commit/eafa6702e1663a02b24b48e3b61ea6252b2a9b40))
* troubleshoot renovate ([c3d9523](https://github.com/open-feature/open-feature-operator/commit/c3d95232d0f1ca6e8c898ffffb165537462fe2e9))
* troubleshoot renovatge ([35054cb](https://github.com/open-feature/open-feature-operator/commit/35054cb6917dcacbafb9fbccb00a85493922f245))
* troubleshoot renvoate ([7ac3c90](https://github.com/open-feature/open-feature-operator/commit/7ac3c90a358baf6f0dd00bd2f7295665ebf46a59))
* update codeowners to use cloud native team ([6133060](https://github.com/open-feature/open-feature-operator/commit/613306011016a3cbb7fbc23a2273aecfd26a3bbf))
* update flagd renovate detection ([#439](https://github.com/open-feature/open-feature-operator/issues/439)) ([3d1540c](https://github.com/open-feature/open-feature-operator/commit/3d1540c67c7d43c69feb61654b7d2a3c8a72a5a1))
* update renovate config to watch the assert yaml directly ([9ef25a0](https://github.com/open-feature/open-feature-operator/commit/9ef25a0abbdeb15666679fd43d4f2c032b825722))
* use renovate to bump flagd version ([#395](https://github.com/open-feature/open-feature-operator/issues/395)) ([fd5b072](https://github.com/open-feature/open-feature-operator/commit/fd5b072214f1c3c74dfc4bc53ca1ff6c14d72ffa))

## [0.2.31](https://github.com/open-feature/open-feature-operator/compare/v0.2.30...v0.2.31) (2023-03-16)


### 📚 Documentation

* fix rendering issue with operator resource config table ([#401](https://github.com/open-feature/open-feature-operator/issues/401)) ([71ea8a6](https://github.com/open-feature/open-feature-operator/commit/71ea8a68bbb97052822552ffce3c498c3da0e52d))


### 🐛 Bug Fixes

* update flagd version ([#402](https://github.com/open-feature/open-feature-operator/issues/402)) ([dc6aa3c](https://github.com/open-feature/open-feature-operator/commit/dc6aa3c3dd9fec6c508b34608384247b63b42eeb))

## [0.2.30](https://github.com/open-feature/open-feature-operator/compare/v0.2.29...v0.2.30) (2023-03-16)


### 📚 Documentation

* add AND operator to sequential commands ([#368](https://github.com/open-feature/open-feature-operator/issues/368)) ([6f73a62](https://github.com/open-feature/open-feature-operator/commit/6f73a6214d87771f9555469fe4d60dbb6d301198))


### ✨ New Features

* enable flagd probes ([#390](https://github.com/open-feature/open-feature-operator/issues/390)) ([41efb15](https://github.com/open-feature/open-feature-operator/commit/41efb155994b3cfb768cc39e59bfc09781c57f2e))
* improve deployment pattern ([#344](https://github.com/open-feature/open-feature-operator/issues/344)) ([572ba96](https://github.com/open-feature/open-feature-operator/commit/572ba961912ada2c07eb6143925d16ab6a6a85a3))


### 🐛 Bug Fixes

* **deps:** update module sigs.k8s.io/controller-runtime to v0.14.5 ([#279](https://github.com/open-feature/open-feature-operator/issues/279)) ([8a80bff](https://github.com/open-feature/open-feature-operator/commit/8a80bff886af404e897e6a247cea2f4c88d88499))


### 🧹 Chore

* add additional sections to the release notes ([4bec5af](https://github.com/open-feature/open-feature-operator/commit/4bec5af5fc5fc589d920f0c17a1213a036b558a0))
* add artifact hub metadata ([#372](https://github.com/open-feature/open-feature-operator/issues/372)) ([c6f539f](https://github.com/open-feature/open-feature-operator/commit/c6f539f5bdd9dc18ac197eb3303d91131e863011))
* **deps:** update dependency open-feature/flagd to v0.4.0 ([#342](https://github.com/open-feature/open-feature-operator/issues/342)) ([0640f46](https://github.com/open-feature/open-feature-operator/commit/0640f469daa3c0adce920bb73e901fe83bc275e7))
* **deps:** update dependency open-feature/flagd to v0.4.1 ([#373](https://github.com/open-feature/open-feature-operator/issues/373)) ([756cf7a](https://github.com/open-feature/open-feature-operator/commit/756cf7a96c05fdfa8ffa2bf933225b84af400e37))
* **deps:** update dependency open-feature/flagd to v0.4.4 ([#400](https://github.com/open-feature/open-feature-operator/issues/400)) ([3e0a666](https://github.com/open-feature/open-feature-operator/commit/3e0a666f2824071c49250a4467d62b96a5af5ee7))
* **deps:** update docker/login-action digest to 219c305 ([#365](https://github.com/open-feature/open-feature-operator/issues/365)) ([ee84954](https://github.com/open-feature/open-feature-operator/commit/ee849546322516019ea19a205c22c4ee38ac36ed))
* **deps:** update docker/metadata-action digest to 766400c ([#267](https://github.com/open-feature/open-feature-operator/issues/267)) ([38a1464](https://github.com/open-feature/open-feature-operator/commit/38a14644e687b928e51d1350f6d57ef9d493330c))
* **deps:** update docker/metadata-action digest to 9ec57ed ([#366](https://github.com/open-feature/open-feature-operator/issues/366)) ([884d444](https://github.com/open-feature/open-feature-operator/commit/884d44422ad7bfa28a8fb88156cd66e252e2eba5))
* **deps:** update gcr.io/kubebuilder/kube-rbac-proxy docker tag to v0.14.0 ([#376](https://github.com/open-feature/open-feature-operator/issues/376)) ([708e4bc](https://github.com/open-feature/open-feature-operator/commit/708e4bc44d8493d4f0aaa7f7036c2b7ecd2efd32))
* **deps:** update ghcr.io/open-feature/flagd docker tag to v0.4.4 ([#381](https://github.com/open-feature/open-feature-operator/issues/381)) ([a253761](https://github.com/open-feature/open-feature-operator/commit/a253761af8565fdcf6e6f9ca92c740f25b4b0620))
* **deps:** update golang docker tag to v1.20.2 ([#374](https://github.com/open-feature/open-feature-operator/issues/374)) ([e2de529](https://github.com/open-feature/open-feature-operator/commit/e2de52997b44835a4a8515e9fd37c976d3539272))
* e2e test for openfeature.dev/enabled annotation set to false ([#375](https://github.com/open-feature/open-feature-operator/issues/375)) ([b03fb14](https://github.com/open-feature/open-feature-operator/commit/b03fb145e317f987727d76b98041fa783e5c2202))
* improve formatting and content ([#384](https://github.com/open-feature/open-feature-operator/issues/384)) ([c5a6a32](https://github.com/open-feature/open-feature-operator/commit/c5a6a32f0ccccc6449fc581de08c283434c1adb6))
* remove unneeded conversion webhooks + introduce unit tests for conversion functions ([#385](https://github.com/open-feature/open-feature-operator/issues/385)) ([dd34801](https://github.com/open-feature/open-feature-operator/commit/dd34801fd71ac4f1e6c0b0f39f78ddf738f5601d))

## [0.2.29](https://github.com/open-feature/open-feature-operator/compare/v0.2.28...v0.2.29) (2023-02-23)


### Features

* add log format configuration options through helm chart ([#346](https://github.com/open-feature/open-feature-operator/issues/346)) ([bcef736](https://github.com/open-feature/open-feature-operator/commit/bcef7368fc4905b351f81f5dfa10eb4c26bf8764))
* Introduced context to the readyz endpoint, added wait to test suite ([#336](https://github.com/open-feature/open-feature-operator/issues/336)) ([ed81c02](https://github.com/open-feature/open-feature-operator/commit/ed81c0284f8d759eb228d3af7030efb0b94ee280))


### Bug Fixes

* Security issues ([#348](https://github.com/open-feature/open-feature-operator/issues/348)) ([5bd0b19](https://github.com/open-feature/open-feature-operator/commit/5bd0b192a5db7f1557e1161e4bb425bbf0e31e2a))
* set defaultTag to INPUT_FLAGD_VERSION ([#332](https://github.com/open-feature/open-feature-operator/issues/332)) ([23547a1](https://github.com/open-feature/open-feature-operator/commit/23547a1e155e0cde2f085882bfd43128681466cd))

## [0.2.28](https://github.com/open-feature/open-feature-operator/compare/v0.2.27...v0.2.28) (2023-01-28)


### Bug Fixes

* mount dirs not files ([#326](https://github.com/open-feature/open-feature-operator/issues/326)) ([089ab3c](https://github.com/open-feature/open-feature-operator/commit/089ab3c48c0937e64060057e43ff07cf8fd47f67))

## [0.2.27](https://github.com/open-feature/open-feature-operator/compare/v0.2.26...v0.2.27) (2023-01-27)


### Features

* default sync provider configuration ([#320](https://github.com/open-feature/open-feature-operator/issues/320)) ([7cba7e1](https://github.com/open-feature/open-feature-operator/commit/7cba7e14c223a083f02ff8313b899583253120f3))


### Bug Fixes

* gave configmaps volume mounts a subpath to allow for multiple mounts ([#321](https://github.com/open-feature/open-feature-operator/issues/321)) ([2ec454c](https://github.com/open-feature/open-feature-operator/commit/2ec454c036149ebeaf34f81cbf4ad7895f0bb995))
* uniqueness of featureflagconfiguration file path ([#323](https://github.com/open-feature/open-feature-operator/issues/323)) ([2b10945](https://github.com/open-feature/open-feature-operator/commit/2b109452893abd053640ffbb9c79b834b78feb7b))

## [0.2.26](https://github.com/open-feature/open-feature-operator/compare/v0.2.25...v0.2.26) (2023-01-26)


### Bug Fixes

* **deps:** update module github.com/open-feature/schemas to v0.2.8 ([#269](https://github.com/open-feature/open-feature-operator/issues/269)) ([ed48060](https://github.com/open-feature/open-feature-operator/commit/ed48060b1f9e591ddadca4f9478728a823e10685))

## [0.2.25](https://github.com/open-feature/open-feature-operator/compare/v0.2.24...v0.2.25) (2023-01-25)


### Features

* Helm configuration ([#304](https://github.com/open-feature/open-feature-operator/issues/304)) ([99edfeb](https://github.com/open-feature/open-feature-operator/commit/99edfeb8c32ada435f830c6799540ebdf3b5fcdd))


### Bug Fixes

* removed duplicate config map generation, resolve permissions issue ([#305](https://github.com/open-feature/open-feature-operator/issues/305)) ([eec16af](https://github.com/open-feature/open-feature-operator/commit/eec16af28eb963a3d0f276d382e808079e663a50))
* update x/net for CVE-2022-41721 ([#301](https://github.com/open-feature/open-feature-operator/issues/301)) ([bbe9837](https://github.com/open-feature/open-feature-operator/commit/bbe983786ff74b59046b95082d79f71089fe2b67))

## [0.2.24](https://github.com/open-feature/open-feature-operator/compare/v0.2.23...v0.2.24) (2023-01-16)


### Features

* backfill flagd-kubernetes-sync cluster role binding on startup ([#295](https://github.com/open-feature/open-feature-operator/pull/295))
* decouple feature flag spec from flagd config ([#276](https://github.com/open-feature/open-feature-operator/pull/276))


### Features

* upgrade flagd to v0.3.0 ([20571e1](https://github.com/open-feature/open-feature-operator/commit/20571e1018e102ffbcf01b2518fcbf8b66a287be))

## [0.2.22](https://github.com/open-feature/open-feature-operator/compare/v0.2.21...v0.2.22) (2022-12-16)


### Bug Fixes

* **deps:** update module go.uber.org/zap to v1.24.0 ([#268](https://github.com/open-feature/open-feature-operator/issues/268)) ([b7bdde8](https://github.com/open-feature/open-feature-operator/commit/b7bdde8944446621751e6ef70e6b0f0646adee21))
* Version fix ([#284](https://github.com/open-feature/open-feature-operator/issues/284)) ([a9c6f15](https://github.com/open-feature/open-feature-operator/commit/a9c6f154589f1e00e60883c229b3ee29d7d2e9aa))

## [0.2.21](https://github.com/open-feature/open-feature-operator/compare/v0.2.20...v0.2.21) (2022-12-16)


### Features

* add ff shortname, commit httpSyncConfiguration ([11e4652](https://github.com/open-feature/open-feature-operator/commit/11e46528fcd06cdc0c8e6f46944656224cd97441))
* introduce configurable resource limits for flagd sidecar ([e4affcf](https://github.com/open-feature/open-feature-operator/commit/e4affcfb0ccf13dc0406ef1c21c2b884a836f71f))


### Bug Fixes

* **deps:** update github.com/open-feature/schemas digest to 302d0fa ([#246](https://github.com/open-feature/open-feature-operator/issues/246)) ([7d22374](https://github.com/open-feature/open-feature-operator/commit/7d22374afb7a5e2e166550544d327ec7b5b3d1bf))
* **deps:** update kubernetes packages to v0.25.4 ([75bab2d](https://github.com/open-feature/open-feature-operator/commit/75bab2d441c945d51f17f0d32195a217072c3c15))
* include release tag in helm charts publishing ([2746716](https://github.com/open-feature/open-feature-operator/commit/27467164dcd05b0220e0857bf79e42d62e7a40a9))

## [0.2.20](https://github.com/open-feature/open-feature-operator/compare/v0.2.19...v0.2.20) (2022-11-18)


### Bug Fixes

* **deps:** update module sigs.k8s.io/controller-runtime to v0.13.1 ([edeffcd](https://github.com/open-feature/open-feature-operator/commit/edeffcd3ef6fe9a8d52d0d5c414512ef8cd80629))

## [0.2.19](https://github.com/open-feature/open-feature-operator/compare/v0.2.18...v0.2.19) (2022-11-15)


### Features

* introduced v1beta1 of featureflagconfiguration CRD with conversion webhook to v1alpha1 ([a45bdef](https://github.com/open-feature/open-feature-operator/commit/a45bdef5eec87738ce731af5825daffeb69eb6cb))
* structured the featureflagconfiguration CRD ([b056c7c](https://github.com/open-feature/open-feature-operator/commit/b056c7cdd76f4653c1a728342687beaa8279e314))

## [0.2.18](https://github.com/open-feature/open-feature-operator/compare/v0.2.17...v0.2.18) (2022-11-10)


### Bug Fixes

* nil pointer dereference ([#216](https://github.com/open-feature/open-feature-operator/issues/216)) ([d975066](https://github.com/open-feature/open-feature-operator/commit/d975066f96a5f9caf8af8d513076480a33943257))

## [0.2.17](https://github.com/open-feature/open-feature-operator/compare/v0.2.16...v0.2.17) (2022-11-07)


### Bug Fixes

* **deps:** update github.com/open-feature/schemas digest to d638ecf ([a984836](https://github.com/open-feature/open-feature-operator/commit/a98483696f467270783858046132f02b3d338ac2))
* for helm issues ([#206](https://github.com/open-feature/open-feature-operator/issues/206)) ([39febd7](https://github.com/open-feature/open-feature-operator/commit/39febd76d1b996afdbc24399bcd08b502621c6cc))

## [0.2.16](https://github.com/open-feature/open-feature-operator/compare/v0.2.15...v0.2.16) (2022-10-27)


### Bug Fixes

* resolve issue with templated DNS name in cert ([65068df](https://github.com/open-feature/open-feature-operator/commit/65068df3019312a965271e50c52bbb90b68665c0))

## [0.2.15](https://github.com/open-feature/open-feature-operator/compare/v0.2.14...v0.2.15) (2022-10-25)


### Bug Fixes

* artifact name and output file ([#187](https://github.com/open-feature/open-feature-operator/issues/187)) ([4dee157](https://github.com/open-feature/open-feature-operator/commit/4dee157d44c20fc925f9e33dbaae16c18f3d9b48))
* remove redundant name ([#189](https://github.com/open-feature/open-feature-operator/issues/189)) ([664bd73](https://github.com/open-feature/open-feature-operator/commit/664bd7314e376b23a01247b5c027c04a9ac26329))

## [0.2.14](https://github.com/open-feature/open-feature-operator/compare/v0.2.13...v0.2.14) (2022-10-25)


### Bug Fixes

* add sbom to ouput name ([#182](https://github.com/open-feature/open-feature-operator/issues/182)) ([5e939a8](https://github.com/open-feature/open-feature-operator/commit/5e939a8f67fbd095c18a6a2172bb856fe61dd173))

## [0.2.13](https://github.com/open-feature/open-feature-operator/compare/v0.2.12...v0.2.13) (2022-10-25)


### Bug Fixes

* set sbom dir ([#180](https://github.com/open-feature/open-feature-operator/issues/180)) ([616272d](https://github.com/open-feature/open-feature-operator/commit/616272d6d693115a22839cf52eb8fd448609ad6c))

## [0.2.12](https://github.com/open-feature/open-feature-operator/compare/v0.2.11...v0.2.12) (2022-10-25)


### Bug Fixes

* set sbom dir ([#178](https://github.com/open-feature/open-feature-operator/issues/178)) ([143adf9](https://github.com/open-feature/open-feature-operator/commit/143adf910fe15a8b8af31dff48743352ab203d83))

## [0.2.11](https://github.com/open-feature/open-feature-operator/compare/v0.2.10...v0.2.11) (2022-10-25)


### Bug Fixes

* Upload sbom ([#175](https://github.com/open-feature/open-feature-operator/issues/175)) ([813c646](https://github.com/open-feature/open-feature-operator/commit/813c6469ecc18101f60c593282ed32d7579f5880))
* Upload sbom by name ([#176](https://github.com/open-feature/open-feature-operator/issues/176)) ([7d0fcd0](https://github.com/open-feature/open-feature-operator/commit/7d0fcd0ba7eeee1b2424189c7e5f5f92bc1fffac))

## [0.2.10](https://github.com/open-feature/open-feature-operator/compare/v0.2.9...v0.2.10) (2022-10-25)


### Bug Fixes

* correcrt needs in asset release ([5ed4571](https://github.com/open-feature/open-feature-operator/commit/5ed45718ca189a15f7cdf4f8ddfc5864f189b1ce))

## [0.2.9](https://github.com/open-feature/open-feature-operator/compare/v0.2.8...v0.2.9) (2022-10-25)


### Bug Fixes

* Package signing should happen in the oci workflow. ([a04a110](https://github.com/open-feature/open-feature-operator/commit/a04a110e29b1725a66d0f4b529741947ebb7c798))

## [0.2.8](https://github.com/open-feature/open-feature-operator/compare/v0.2.7...v0.2.8) (2022-10-25)


### Bug Fixes

* package signing fixes ([36597f4](https://github.com/open-feature/open-feature-operator/commit/36597f484c85effd6a993f44b97fcd541d34c515))

## [0.2.7](https://github.com/open-feature/open-feature-operator/compare/v0.2.6...v0.2.7) (2022-10-25)


### Features

* adding artifacthub information ([#144](https://github.com/open-feature/open-feature-operator/issues/144)) ([65a5244](https://github.com/open-feature/open-feature-operator/commit/65a524445d1db8bb5608b88282a4d97a9bb6b74f))
* builds helm chart ([#137](https://github.com/open-feature/open-feature-operator/issues/137)) ([1525421](https://github.com/open-feature/open-feature-operator/commit/1525421229d43b17636dddb65d7b124e6477fe79))

## [0.2.7](https://github.com/open-feature/open-feature-operator/compare/v0.2.6...v0.2.7) (2022-10-24)


### Features

* adding artifacthub information ([#144](https://github.com/open-feature/open-feature-operator/issues/144)) ([65a5244](https://github.com/open-feature/open-feature-operator/commit/65a524445d1db8bb5608b88282a4d97a9bb6b74f))
* builds helm chart ([#137](https://github.com/open-feature/open-feature-operator/issues/137)) ([1525421](https://github.com/open-feature/open-feature-operator/commit/1525421229d43b17636dddb65d7b124e6477fe79))

## [0.2.6](https://github.com/open-feature/open-feature-operator/compare/v0.2.5...v0.2.6) (2022-10-24)


### Features

* adding artifacthub information ([#144](https://github.com/open-feature/open-feature-operator/issues/144)) ([65a5244](https://github.com/open-feature/open-feature-operator/commit/65a524445d1db8bb5608b88282a4d97a9bb6b74f))
* builds helm chart ([#137](https://github.com/open-feature/open-feature-operator/issues/137)) ([1525421](https://github.com/open-feature/open-feature-operator/commit/1525421229d43b17636dddb65d7b124e6477fe79))


### Bug Fixes

* CVE-2022-32149 ([015c19a](https://github.com/open-feature/open-feature-operator/commit/015c19ac4455673902c365111816b021f893c485))

## [0.2.6](https://github.com/open-feature/open-feature-operator/compare/v0.2.5...v0.2.6) (2022-10-20)


### Bug Fixes

* CVE-2022-32149 ([015c19a](https://github.com/open-feature/open-feature-operator/commit/015c19ac4455673902c365111816b021f893c485))

## [0.2.5](https://github.com/open-feature/open-feature-operator/compare/v0.2.4...v0.2.5) (2022-10-19)


### Features

* stop creation and mounting of flagd-config config map in case of kubernetes sync-provider ([#126](https://github.com/open-feature/open-feature-operator/issues/126)) ([a1d9fe2](https://github.com/open-feature/open-feature-operator/commit/a1d9fe276a37259d01e6ed6239c0ebcd3a1e6611))

## [0.2.4](https://github.com/open-feature/open-feature-operator/compare/v0.2.3...v0.2.4) (2022-10-18)


### Bug Fixes

* build and push to docker registry with tag as current release ([#123](https://github.com/open-feature/open-feature-operator/issues/123)) ([d4abda1](https://github.com/open-feature/open-feature-operator/commit/d4abda119e4a7c2dab7a2e0d335d44b1df07ec62))

## [0.2.3](https://github.com/open-feature/open-feature-operator/compare/v0.2.2...v0.2.3) (2022-10-18)


### Bug Fixes

* build and push to docker registry on tag creation ([#121](https://github.com/open-feature/open-feature-operator/issues/121)) ([27c6f9c](https://github.com/open-feature/open-feature-operator/commit/27c6f9cbc298fb8bf578464e4c3f9f07402b87ab))

## [0.2.2](https://github.com/open-feature/open-feature-operator/compare/v0.2.1...v0.2.2) (2022-10-14)


### Bug Fixes

* bump flagd version to include change detection fix ([421cab6](https://github.com/open-feature/open-feature-operator/commit/421cab651f6ebe2ece1380fda7dc24d92838d6b5))

## [0.2.1](https://github.com/open-feature/open-feature-operator/compare/v0.2.0...v0.2.1) (2022-10-13)


### Features

* metrics ([#111](https://github.com/open-feature/open-feature-operator/issues/111)) ([6016669](https://github.com/open-feature/open-feature-operator/commit/6016669ec46984d127951ee5d0ff02e7685f4d80))
* pr github action workflow ([#96](https://github.com/open-feature/open-feature-operator/issues/96)) ([a719f8a](https://github.com/open-feature/open-feature-operator/commit/a719f8a33abc9b9599987314282cc4e7ac202d67))


### Bug Fixes

* include assets in release ([#109](https://github.com/open-feature/open-feature-operator/issues/109)) ([b835abb](https://github.com/open-feature/open-feature-operator/commit/b835abb48ae8ca3c9c63abd51ae5614a4068c003))

## [0.2.0](https://github.com/open-feature/open-feature-operator/compare/v0.1.1...v0.2.0) (2022-10-10)


### ⚠ BREAKING CHANGES

* bump flagd version to 0.2.0 (connect refactor) (#97)

### Features

* bump flagd version to 0.2.0 (connect refactor) ([#97](https://github.com/open-feature/open-feature-operator/issues/97)) ([8118b9f](https://github.com/open-feature/open-feature-operator/commit/8118b9fcbaf0d3c66d6869369add645e388989de))


### Bug Fixes

* upgrade dependencies with vulnerabilities ([#90](https://github.com/open-feature/open-feature-operator/issues/90)) ([58cdd4e](https://github.com/open-feature/open-feature-operator/commit/58cdd4ee7c6989e44258bad3e9ed75a3bb465cae))
