pipeline{
  agent any
      stages {
         stage("maven build"){
           when{
             branch 'develop'
            }
             steps{ 
                 echo "maven build.........."  
             }
          }
         stage("sonar analysis"){
           when{
             branch 'develop'
            }
             steps{ 
                 echo "sonar analysis..........."  
             }
          }
         stage("deploy to dev"){
           when{
             branch 'develop'
            }
             steps{ 
                 echo "deploying to development..........."  
             }
          }
         stage("deploy to qa"){
           when{
             branch 'test'
            }
             steps{ 
                 echo "deploying to qa..........."  
             }
          }
         stage("deploy to prod"){
           when{
             branch 'main'
            }
             steps{ 
                 echo "deploying to prod..........."  
             }
          }
        }
      }
