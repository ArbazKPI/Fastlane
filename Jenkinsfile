#! groovy

pipeline {
    agent any

    stages{

    stage('Setup') {
  steps {
    echo "Setup"

    sh "su - Arbaz -p KPITECH"

    sh "sudo apt-get install build-essential"

    sh "sudo gem install bundler"

    sh "sudo bundle install"

    sh "bundle exec fastlane beta"
  }
}
}
}