# Gradle common includes
A library of commonly used gradle snippets that can be included in other gradle build files with `apply from: '[URL]'`

## versioning.gradle
Provides functionality for getting version numbers from git. Almost all functions require git tags to be useful with the exception of `getCommitCountTotal` & `getLatestCommitHash`

Example: If there are a total of 10 commits and you tag the first commit as `1.0` then running `getPrettyVersionName` will produce the output "1.0.9"
