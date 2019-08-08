properties([ disableConcurrentBuilds(),buildDiscarder(logRotator(numToKeepStr:'10')), pipelineTriggers([githubPush()]) ])

node{
    
    checkout scm
}


stage('deployment'){
    sh 'ansible-playbook deploy.yml '    
    } 
