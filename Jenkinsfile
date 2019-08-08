properties([ disableConcurrentBuilds(),buildDiscarder(logRotator(numToKeepStr:'10')), pipelineTriggers([githubPush()]) ])

pipeline{
 agent any

stages {
stage('deployment'){

sh 'ansible-playbook deploy.yml'     

    } 
   }
}
