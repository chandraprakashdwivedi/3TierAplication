properties([ disableConcurrentBuilds(),buildDiscarder(logRotator(numToKeepStr:'10')), pipelineTriggers([githubPush()]) ])


stage('deployment'){
deleteDir()
checkout scm

sh 'ansible-playbook deploy.yml'     

 } 
