pipeline { 
     agent any
     stages{
       stage('Pulling GIT') {
             steps {
		script {
                  git 'https://github.com/Oumayma-b/LContinue.git'
            }
        }        
     }
        stage('Build') 
        { 
        steps{ 
             script{
                   
              sh "ansible-playbook ansible/build.yml -i ansible/inventory/host.yml"

             }
          }
        }
     }
}
