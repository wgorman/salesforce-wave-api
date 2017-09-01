#!/usr/bin/env groovy

// Use the default version of the jenkins-pipelines plugin
@Library("corvana-jenkins-pipelines") _

pods.standard {
   checkout scm
   stage('Build') {
        mvn('deploy -DskipTests=true', './pom.xml', null)
   }
}
