# sonarqube-findbug-integration
Findbugs-
works on .class files.
Findbugs always works on btye code,that means it is going to analyze your byte code and then it is going to report the issue,but sonar way it is going to take the source code that is java files and it will start analyzing ur project.
Findbugs works on byte code,sonarway works on .java files.

you can also use debug mode to analyze what is being done and what profile is beaing used.

Add folloing entry in build.gradle file in ordet to add Findbugs plugin.
sonarqube {

properties {

    property "sonar.projectName" , "FindBug Testing"
	property "sonar.projectKey" , "FindBug"
	property "sonar.host.url" , "http://localhost:9000/"
	property "sonar.scm.disabled" , "true"    // As not using any SCM tools,but using then marked as false and give SCM url.

}
}


