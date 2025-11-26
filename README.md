# Task 8 – Java Maven Build with Jenkins

This repository contains a simple Java "HelloWorld" application built using Maven
and a Jenkins Freestyle job, as required for DevOps Internship Task 8.

## Contents
- `src/main/java/HelloWorld.java` – basic Java program printing "Hello, Jenkins + Maven!"
- `pom.xml` – Maven build configuration (compiler plugin, Java 1.8)
- `screenshots/build-success.png` – Jenkins console output showing `BUILD SUCCESS`

## Jenkins Job Setup (Summary)
1. Ran Jenkins via Docker:
   `docker run -p 8080:8080 jenkins/jenkins:lts`
2. Configured Maven under **Manage Jenkins → Global Tool Configuration**.
3. Created Freestyle job `hello-java-maven-build`.
4. Set **Source Code Management** to Git repo: this repository.
5. Added build step **Invoke top-level Maven targets** with goal `clean package`.
6. Clicked **Build Now** and verified `BUILD SUCCESS` in console output.

This completes Task 8.
