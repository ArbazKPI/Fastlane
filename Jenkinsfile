#! groovy

pipeline {
    agent any

    stages{

    stage('Setup') {
  steps {

                sh "bundle install"

    //change permission of gradlew and Gemfile
                sh "chmod +x Jenkinsfile"
                //sh "chmod +x Gemfile"
                sh "chmod +x gradlew"

                sh "sudo chmod +w /var/lib"

                
                //build and upload to firebase
                sh "fastlane beta"
    

        
        
        
        

        

        
  }
}
}
}