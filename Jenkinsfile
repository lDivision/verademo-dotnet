pipeline {
  agent any

  stages {
    stage ('Dotnet Restore') {
      steps {
        script {
          def slnFile = sh(script: 'find . -name "*.sln"', returnStdout: true).trim()
          sh "dotnet restore ${slnFile}"
        }
      }
    }
  }
}
