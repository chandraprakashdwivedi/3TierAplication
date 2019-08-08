//workspace = "${env.WORKSPACE}"
def workspace = pwd()

properties([ disableConcurrentBuilds(), pipelineTriggers([githubPush()]) ]) 
 
node{
      deleteDir()
      checkout scm

     stage('deploying stack'){
      echo $workspace
      sh 'ansible-playbook deploy.yml'
      } 
     
}
