> expo-release-please-example

Setting up [release-please][release-please-github-repo] with basic Expo app.

# Example of Expo app setup with please-release

- Minimal Expo app based on quick start section of Expo [documentation][expo-app-get-started]. Bootstrapped with yarn 3. Heads up, your versions might differ based on various factors.

```shell
yarn dlx create-expo-app expo-release-please-example
```

and

```shell
yarn dlx expo install react-native-web@~0.18.9 react-dom@18.1.0 @expo/webpack-config@^0.17.2
```

- Setting up [release-please-action][release-please-github-action-repo] for `expo` release type strategy.

- Using arbitrary file update [feature][release-please-doc-arbitrary-file-update] inside this [README.md][readme-code-arbitrary-file-update] to display current version **v2.0.0** (note inline comment) <!-- x-release-please-version -->

- This is [initial][version-pr-initial] first PR introduced by release-please.
- This is [patch][version-pr-patch] PR with fixes.
- This is [breaking][version-pr-major] PR with breaking fixes.
- This is [feature][version-pr-feat] PR with new feature.

### Note on existing repo versioning

This example assumes `release-please` being used from the initial app bootstrap. If you already have an app running and want to start with some existing version consider using bootstrapping `release-please` with [.release-please-manifest.json][release-please-initial-version] file.
For this package context of this file **might** look something like.

```json
{
  "packages": {
    ".": "3.4.5"
  }
}
```

[expo-app-get-started]: https://docs.expo.dev
[release-please-github-repo]: https://github.com/googleapis/release-please
[release-please-github-action-repo]: https://github.com/google-github-actions/release-please-action
[release-please-doc-arbitrary-file-update]: https://github.com/googleapis/release-please/blob/main/docs/customizing.md#updating-arbitrary-json-files
[version-pr-initial]: https://github.com/dmi3y/expo-release-please-example/pull/1/files
[readme-code-arbitrary-file-update]: https://github.com/dmi3y/expo-release-please-example/blob/main/README.md?plain=1#L19
[version-pr-patch]: https://github.com/dmi3y/expo-release-please-example/pull/2
[release-please-initial-version]: https://github.com/googleapis/release-please/blob/main/docs/manifest-releaser.md#initial-version
[version-pr-major]: https://github.com/dmi3y/expo-release-please-example/pull/3
[version-pr-feat]: https://github.com/dmi3y/expo-release-please-example/pull/4
