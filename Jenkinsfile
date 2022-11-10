#! groovy

pipeline {
    agent any

    stages{

    stage('Setup') {
  steps {
    echo "Setup"

    
  
    
    sh "bundle install"

    sh "bundle exec fastlane beta"
  }
}
}
}