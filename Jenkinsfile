//properties([ disableConcurrentBuilds(),buildDiscarder(logRotator(numToKeepStr:'10')), pipelineTriggers([githubPush()]) ])



stage('deployment'){

sh 'ansible-playbook deploy.yml -vvv'    

    } 
