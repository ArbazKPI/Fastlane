#! groovy

pipeline {
    agent any

    stages{

    stage('Setup') {
  steps {
    echo "Setup"



    sh "bundle exec fastlane beta"
  }
}
}
}