# How to run ?

## Run test and coverage with jacoco
```
$./gradlew clean test
```

## Run coverage report with Jacoco
```
$./gradlew jacocoTestReport
```

* HTML report in `build/reports/jacoco/test/html/index.html`
* Jacoco result in `build/jacoco/test.exec`

## Build 
```
$./gradlew build
```

## Start Development server
```
$gradlew bootRun
```
## Working with SonarQube

```
$gradlew sonarqube
```