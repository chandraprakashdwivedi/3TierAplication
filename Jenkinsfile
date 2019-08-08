properties([ disableConcurrentBuilds(),buildDiscarder(logRotator(numToKeepStr:'10')), pipelineTriggers([githubPush()]) ])

node{
      deleteDir()
      checkout scm
}
stage('deployment'){

sh 'ansible-playbook deploy.yml'     

 } 
