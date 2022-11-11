#! groovy

pipeline {
    agent any

    stages{

    stage('Setup') {
  steps {

    environment {

      Root_password = 'KPITECH'
    }

            

                sh "echo "Root_password" | sudo -S sleep 1 && sudo su - Arbaz"
                sh "bundle install"

    //change permission of gradlew and Gemfile
                sh "chmod +x Jenkinsfile"
                //sh "chmod +x Gemfile"
                sh "chmod +x gradlew"

                sh "chmod +w /var/lib"

                
                //build and upload to firebase
                sh "fastlane beta"
    

        
        
        
        

        

        
  }
}
}
}