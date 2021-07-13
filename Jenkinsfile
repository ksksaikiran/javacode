pipeline{
  agent any
    stages{
      stage("git checkout"){
        steps{
          echo "pulling the code"
          git "https://www.github.com/ksksaikiran/javacode.git"
         }
      }
       stage("Maven validation"){
        steps{
          echo "validating  the code"
            sh "mvn validate"
            sh "mvn package"
         }
      }
    }
}
