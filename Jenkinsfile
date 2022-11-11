#! groovy

pipeline {
    agent any

    stages{

    stage('Setup') {
  steps {

    //change permission of gradlew and Gemfile
                sh "chmod +x fastlane-1/Jenkinsfile"
                //sh "chmod +x Gemfile"

                
                //build and upload to firebase
                sh "fastlane beta"
    

        
        
        
        

        

        
  }
}
}
}