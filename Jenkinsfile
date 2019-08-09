//workspace = "${env.WORKSPACE}"
workspace = '/var/lib/jenkins/jobs/3tierApp'
 
properties([ disableConcurrentBuilds(), pipelineTriggers([githubPush()]) ]) 
 
node{
      deleteDir()
      checkout scm

     stage('deploying stack'){
      sh 'ansible-playbook deploy.yml -vvv'
      } 
     
}
