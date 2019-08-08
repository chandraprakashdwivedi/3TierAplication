properties([ disableConcurrentBuilds(), pipelineTriggers([githubPush()]) ]) 
 
node{
      deleteDir()
      checkout scm

     stage('adding plugin'){

      sh 'ansible-playbook deploy.yml'

      } 
     
}
