# Gradle common includes
A library of commonly used gradle snippets that can be included in other gradle build files with `apply from: '[URL]'`

## checkstyle.gradle
Performs checks on code based on checkstyle config file provided by the gradle property `CHECKSTYLE_CONFIG`

To configure your checkstyle file edit your `gradle.properties` and add the above property. E.g. `CHECKSTYLE_CONFIG=checkstyle.xml`. This property is relative to the build.gradle in which you apply checkstyle.gradle to. 

## versioning.gradle
Provides functionality for getting version numbers from git. Almost all functions require git tags to be useful with the exception of `getCommitCountTotal` & `getLatestCommitHash`

Example: If there are a total of 10 commits and you tag the first commit as `1.0` then running `getPrettyVersionName` will produce the output "1.0.9"
