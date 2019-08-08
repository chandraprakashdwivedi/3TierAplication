properties([ disableConcurrentBuilds(),buildDiscarder(logRotator(numToKeepStr:'10')), pipelineTriggers([githubPush()]) ])


stage('deployment'){
checkout scm

sh 'ansible-playbook deploy.yml'     

 } 
