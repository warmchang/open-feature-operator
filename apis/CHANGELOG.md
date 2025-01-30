# Changelog

## [0.2.46](https://github.com/warmchang/open-feature-operator/compare/apis-v0.2.45...apis/v0.2.46) (2025-01-30)


### ✨ New Features

* add `flagd` CRD with ingress support ([#633](https://github.com/warmchang/open-feature-operator/issues/633)) ([b0b99a7](https://github.com/warmchang/open-feature-operator/commit/b0b99a7d101fb7e281394acd0d8b22a16546708f))
* add gateway api support ([#725](https://github.com/warmchang/open-feature-operator/issues/725)) ([b393a26](https://github.com/warmchang/open-feature-operator/commit/b393a2669c05d58afe453867401f8d697464b145))
* added interval to the openfeature api source ([#619](https://github.com/warmchang/open-feature-operator/issues/619)) ([18ac733](https://github.com/warmchang/open-feature-operator/commit/18ac7331916f5fa19b2f0c8d2fe34f7ba9f1e595))
* introduce new CRD for in-process evaluation ([#632](https://github.com/warmchang/open-feature-operator/issues/632)) ([51db913](https://github.com/warmchang/open-feature-operator/commit/51db913bc708cc60f00e430e372b68c28c7cbda2))
* Introduce v1beta1 API version ([#535](https://github.com/warmchang/open-feature-operator/issues/535)) ([3acd492](https://github.com/warmchang/open-feature-operator/commit/3acd49289a40e8f07fd20aad46185ac42ceb1b7a))
* introduce v1beta1/common package ([#547](https://github.com/warmchang/open-feature-operator/issues/547)) ([cdc4af4](https://github.com/warmchang/open-feature-operator/commit/cdc4af495f370da7165fd67ad9ef54ccf74be3bf))
* introduce validating webhook for FeatureFlag CR ([#622](https://github.com/warmchang/open-feature-operator/issues/622)) ([c4831a3](https://github.com/warmchang/open-feature-operator/commit/c4831a3cdc00aec36f3fe9bec9abceafba1f8aa8))
* prepare apis for v1beta1 controllers onboarding ([#549](https://github.com/warmchang/open-feature-operator/issues/549)) ([e3c8b42](https://github.com/warmchang/open-feature-operator/commit/e3c8b4290be99d78b88ffef686531a38b97e61be))
* release APIs and Operator independently ([#541](https://github.com/warmchang/open-feature-operator/issues/541)) ([7b1af42](https://github.com/warmchang/open-feature-operator/commit/7b1af42ac41e63ccbb1820b31f579ffea679cff6))


### 🐛 Bug Fixes

* **deps:** update module github.com/stretchr/testify to v1.9.0 ([#671](https://github.com/warmchang/open-feature-operator/issues/671)) ([1d2713d](https://github.com/warmchang/open-feature-operator/commit/1d2713dad6381e56aa3b552c33e1cb3513574a6e))
* flagd environment variables missing prefix ([#730](https://github.com/warmchang/open-feature-operator/issues/730)) ([0aa61ec](https://github.com/warmchang/open-feature-operator/commit/0aa61ec1419ec1d99f3c875dd6526ec8ca8e6014))
* flagd mgmt port setting ignored ([#588](https://github.com/warmchang/open-feature-operator/issues/588)) ([1444328](https://github.com/warmchang/open-feature-operator/commit/1444328691450ee3967d862eebf3a293b4f9fe7c))
* flagd path defaults ([#658](https://github.com/warmchang/open-feature-operator/issues/658)) ([aef1010](https://github.com/warmchang/open-feature-operator/commit/aef1010dff162e8d232942e642c68e3e9ba3f35f))
* include parameters with default values to envVars ([#648](https://github.com/warmchang/open-feature-operator/issues/648)) ([4f0477c](https://github.com/warmchang/open-feature-operator/commit/4f0477c8e0da571a1cf11e4ac8b57dba3d98efe2))
* Revert "chore: release apis 0.2.38" ([#557](https://github.com/warmchang/open-feature-operator/issues/557)) ([ccb8c1d](https://github.com/warmchang/open-feature-operator/commit/ccb8c1d6e12aa36e33239fd96bebbc57fc4ea3bc))


### 🧹 Chore

* adapt API for sidecar image and tag restriction ([#552](https://github.com/warmchang/open-feature-operator/issues/552)) ([726a7f7](https://github.com/warmchang/open-feature-operator/commit/726a7f7149067d2e2696f746a236151fbb67808c))
* adapt shortcuts for custom resources ([#551](https://github.com/warmchang/open-feature-operator/issues/551)) ([61c77c0](https://github.com/warmchang/open-feature-operator/commit/61c77c0c137ec624892c9738ee45828a137f6823))
* bump go to 1.21 ([#604](https://github.com/warmchang/open-feature-operator/issues/604)) ([73d6319](https://github.com/warmchang/open-feature-operator/commit/73d6319820220fc114cdfc7d72f8c2327a35ec37))
* bump k8s libs ([#644](https://github.com/warmchang/open-feature-operator/issues/644)) ([a18d272](https://github.com/warmchang/open-feature-operator/commit/a18d27270eeb9eb7aaccd9e6fb368a55b94f98ba))
* bump operator builder tools versions ([#626](https://github.com/warmchang/open-feature-operator/issues/626)) ([918a697](https://github.com/warmchang/open-feature-operator/commit/918a69732fabb34af2f83ca8f650e433e87d0212))
* clean up unused API code after moving to v1beta1 ([#543](https://github.com/warmchang/open-feature-operator/issues/543)) ([1287b07](https://github.com/warmchang/open-feature-operator/commit/1287b0785fd99cb8bfeaf9fe112aa8a0ed6f5cf9))
* **deps:** update open-feature/flagd ([#670](https://github.com/warmchang/open-feature-operator/issues/670)) ([1174a1b](https://github.com/warmchang/open-feature-operator/commit/1174a1b277c1f335b5f73ee76e0c111fd16ace4b))
* **deps:** update open-feature/flagd ([#689](https://github.com/warmchang/open-feature-operator/issues/689)) ([0d331a9](https://github.com/warmchang/open-feature-operator/commit/0d331a9bc5db752cb3aa49f7ce5afc0830f115fe))
* fix file source documentation ([#556](https://github.com/warmchang/open-feature-operator/issues/556)) ([318c52d](https://github.com/warmchang/open-feature-operator/commit/318c52d2ba38dbfee6deb3f06d3392dc14d80a6c))
* refactor code to decrease complexity ([#554](https://github.com/warmchang/open-feature-operator/issues/554)) ([17a547f](https://github.com/warmchang/open-feature-operator/commit/17a547f88595cb6c177ca93e1a8b4ad49f3c1a5f))
* release apis 0.2.37 ([#544](https://github.com/warmchang/open-feature-operator/issues/544)) ([854e72d](https://github.com/warmchang/open-feature-operator/commit/854e72d964fce51082220a60fc8a7319676e49c3))
* release apis 0.2.38 ([#548](https://github.com/warmchang/open-feature-operator/issues/548)) ([c6165d4](https://github.com/warmchang/open-feature-operator/commit/c6165d426b5be2af89e03695d24fe0b802fb1fe2))
* release apis 0.2.38 ([#558](https://github.com/warmchang/open-feature-operator/issues/558)) ([4ecbc9b](https://github.com/warmchang/open-feature-operator/commit/4ecbc9b8eeac4e1e86c0f4e11ffedf3dbc376f9a))
* release apis 0.2.38 ([#560](https://github.com/warmchang/open-feature-operator/issues/560)) ([069e275](https://github.com/warmchang/open-feature-operator/commit/069e2754210d1a71bc5b70c0d4e6e193f62a7bcb))
* release apis 0.2.39 ([#590](https://github.com/warmchang/open-feature-operator/issues/590)) ([c53a72b](https://github.com/warmchang/open-feature-operator/commit/c53a72b0d4f0ecbb6f839ae1af54621f4c152f42))
* release apis 0.2.40 ([#620](https://github.com/warmchang/open-feature-operator/issues/620)) ([e39e763](https://github.com/warmchang/open-feature-operator/commit/e39e7638a1cc7985e665229303f18dcb57b4b95a))
* release apis 0.2.41 ([#627](https://github.com/warmchang/open-feature-operator/issues/627)) ([546635e](https://github.com/warmchang/open-feature-operator/commit/546635e6d486fd0dbc4aba985e43a928918fd1f4))
* release apis 0.2.42 ([#650](https://github.com/warmchang/open-feature-operator/issues/650)) ([b6cd29f](https://github.com/warmchang/open-feature-operator/commit/b6cd29f787650f6a85f9799fa0c54464dcef58f5))
* release apis 0.2.43 ([#660](https://github.com/warmchang/open-feature-operator/issues/660)) ([aed8ba1](https://github.com/warmchang/open-feature-operator/commit/aed8ba19ffd00f202cdfa980ef063bae49468faa))
* release apis 0.2.44 ([#688](https://github.com/warmchang/open-feature-operator/issues/688)) ([9997ea4](https://github.com/warmchang/open-feature-operator/commit/9997ea443ecc025afd7aff2e33e92fb05acb3b1a))
* release apis 0.2.45 ([#727](https://github.com/warmchang/open-feature-operator/issues/727)) ([dbe1222](https://github.com/warmchang/open-feature-operator/commit/dbe12227bc551dcda472b6c1afedb57321852e33))
* revert recent release ([#559](https://github.com/warmchang/open-feature-operator/issues/559)) ([f7c79e4](https://github.com/warmchang/open-feature-operator/commit/f7c79e4c6f5a5dee05d7db1796bfb9891dbd53a0))
* use github-action for golangci-lint workflow ([#538](https://github.com/warmchang/open-feature-operator/issues/538)) ([a97d336](https://github.com/warmchang/open-feature-operator/commit/a97d336468d5a9b50662f4979784c8388ec10ec1))


### 📚 Documentation

* require hosts, mention host-less rules ([#659](https://github.com/warmchang/open-feature-operator/issues/659)) ([dcab14a](https://github.com/warmchang/open-feature-operator/commit/dcab14a2c55ada5f1df34b3ed164c8b334877b68))
