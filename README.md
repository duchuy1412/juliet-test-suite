# Juliet Test Suite

A collection of test cases in the Java language. It contains examples for 112 different CWEs. 
The test suite is taken from [NIST website](https://samate.nist.gov/SRD/testsuite.php)

This repository add alternative build integration : Gradle and Maven

## Gradle

```
gradle build
```

## Maven

```
mvn compile
```
# SonarLint (Sonarqube)

Vì bộ test gồm rất nhiều file + điều kiện không đủ => nhóm chọn 1 CWE trong số 112 CWEs để chạy công cụ SonarLint

CWE23_Relative_Path_Traversal bao gồm 724 files

## Kết quả

SonarLint tìm thấy 9729 issues sau khi analyze 724 files
![](https://github.com/duchuy1412/juliet-test-suite/blob/master/Sonarqube.PNG "kết quả")

![](https://github.com/duchuy1412/juliet-test-suite/blob/master/sonartime.PNG "thời gian chạy")
