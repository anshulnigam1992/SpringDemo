node {
   stage('clean') {
        sh "chmod +x gradlew"
        sh "./gradlew clean"
    }

    

    stage('BUILD') {
        sh "./gradlew bootRepackage buildDocker -Pprod  -PbuildNumber=${env.BUILD_ID}  -x test"
    }

  


   
 
   
  
}
