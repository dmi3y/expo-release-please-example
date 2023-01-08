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

- Using arbitrary file update [feature][release-please-doc-arbitrary-file-update] inside this [README.md][readme-code-arbitrary-file-update] to display current version v1.0.0 <!-- x-release-please-start-version --> (note inline comment)

- This is [first][initial-version-pr] PR introduced by release-please.

[expo-app-get-started]: https://docs.expo.dev
[release-please-github-repo]: https://github.com/googleapis/release-please
[release-please-github-action-repo]: https://github.com/google-github-actions/release-please-action
[release-please-doc-arbitrary-file-update]: https://github.com/googleapis/release-please/blob/main/docs/customizing.md#updating-arbitrary-json-files
[initial-version-pr]: https://github.com/dmi3y/expo-release-please-example/pull/1/files
[readme-code-arbitrary-file-update]: https://github.com/dmi3y/expo-release-please-example/blob/main/README.md?plain=1#L19
