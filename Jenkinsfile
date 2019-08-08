properties([ disableConcurrentBuilds(),buildDiscarder(logRotator(numToKeepStr:'10')), pipelineTriggers([githubPush()]) )]

node('master'){
      deleteDir()
      checkout scm
}
stage('deployment'){

sh' ansible-playbook deploy.yml'     

 } 
