#! groovy

pipeline {
    agent any

    stages{

    stage('Setup') {
  steps {
    echo "Setup"

        sh "echo <KPITECH> | su - Arbaz"
        
        
        sh "gem install bundler"
        
        sh "bundle config set --local path 'vendor/bundle'"
        
        sh "bundle check || bundle install --jobs=4 --retry=3"

        sh "bundle exec fastlane beta"

        
  }
}
}
}