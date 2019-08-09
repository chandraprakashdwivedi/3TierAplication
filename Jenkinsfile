//workspace = "${env.WORKSPACE}"
def workspace = "/var/lib/jenkins/jobs/3tierApp"
 
properties([ disableConcurrentBuilds(), pipelineTriggers([githubPush()]) ]) 
 
node{
      deleteDir()
      checkout scm

     stage('deploying stack'){
       sh "echo ${workspace}"
      sh 'ansible-playbook deploy.yml -vvv'
      } 
     
}
