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

# So sánh PMD Java và SonarLint (Sonarqube)
Với cùng 1 Test Suite mà nhóm chọn để thử nghiệm với 2 tool trên: **CWE23_Relative_Path_Traversal**
![](/pmd.PNG "kết quả của PMD")

![](/Sonarqube.PNG "Kết quả của SonarLint")

PMD có thời gian chạy nhanh hơn, nhưng số issue tìm được lại ít hơn SonarLint (SonarLint cho kết quả 9729 issues, PMD cho 5878 kết quả)

Vậy SonarLint được đánh giá cao hơn vì nó đã bao gồm các quy tắc có trong PMD
