pipeline {
  agent any
  stages { 
      stage('Cloning our Git') { 
        steps { 
          git 'https://github.com/Ashok7867/demo.git' 
        }
      }
  
      stage('Building our image') {
        steps { 
          script { 
            dockerImage = docker.build + ":$BUILD_NUMBER" 
          }
        }
      }
  }
}
