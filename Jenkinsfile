#! groovy

pipeline {
    agent any

    stages{

    stage('Setup') {
  steps {
    echo "Setup"

        sh "su - Arbaz <<! >/dev/null 2>&1
        KPITECH
        
        gem install bundler
        
        bundle config set --local path 'vendor/bundle'
        
        bundle check || bundle install --jobs=4 --retry=3

        bundle exec fastlane beta

        !"
  }
}
}
}