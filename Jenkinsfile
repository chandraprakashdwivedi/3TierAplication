properties([ disableConcurrentBuilds(),buildDiscarder(logRotator(numToKeepStr:'10')), pipelineTriggers([githubPush()]) ])

node{
    agent none
    checkout scm
}


stage('deployment'){
    sh 'ansible-playbook deploy.yml '    
    } 
