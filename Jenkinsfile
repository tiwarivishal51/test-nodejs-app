pipeline { 
   agent {
        docker {
            image 'node:6-alpine'
            args '-p 3000:3000'
        }

   stages {
   
     stage('Install Dependencies') { 
        steps { 
           bat 'npm install' 
        }
     }
     
     stage('Test') { 
        steps { 
           bat 'echo "testing application..."'
        }
      }

         stage("Deploy application") { 
         steps { 
           bat 'echo "deploying application..."'
         }

     }
  
   	}

   }
