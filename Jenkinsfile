//workspace = "${env.WORKSPACE}"
def workspace = pwd()

properties([ disableConcurrentBuilds(), pipelineTriggers([githubPush()]) ]) 
 
node{
      deleteDir()
      checkout scm

     stage('deploying stack'){
      sh 'echo $workspace'
      sh 'ansible-playbook deploy.yml'
      } 
     
}
