#! groovy

pipeline {
    agent any

    stages{

    stage('Setup') {
  steps {
    echo "Setup"

    sh "sudo -i apt-get install build-essential"

    sh "gem install bundler"

    sh "sudo bundle install"

    sh "bundle exec fastlane beta"
  }
}
}
}