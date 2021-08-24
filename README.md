[![CICD](https://github.com/tamilselvansellamuthu/mywebsite/actions/workflows/CICD.yml/badge.svg?branch=main)](https://github.com/tamilselvansellamuthu/mywebsite/actions/workflows/CICD.yml)
# mywebsite

Sample ASP .Net Core application.

.github/workflows/CICD.yml has following steps.(run steps in widows-latest runner.)

1) setup sonar.
  1.1 setup JDK 11.
  1.2 checkout code.
  1.3 run sonarqube scanner  
2) add msbuild path
3) run msbuild
4) package dotnet application as Nuget Package.
5) push Nuget package to Nexus/GitHub Packages.
6) run nunit test cases included.
7) publish deployment artifacts to release.
8) push the deployment artifacts to Nexus/GitHub Packages.
9) deploy the packages to IIS server.
