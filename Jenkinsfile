#! groovy

pipeline {
    agent any

    stages{

    stage('Setup') {
  steps {
    echo "Setup"
    // Install bundler in order to use fastlane
    sh "gem install bundler"
    // set the local path for bundles in vendor/bundle
    sh "bundle config set --local path 'vendor/bundle'"
    
    sh "bundle install"
  }
}


stage('Build') {
  steps {
    echo "Building"
    sh "bundle exec fastlane beta"
  }
}

}
}