pipeline {
  agent any

  stages {
    stage ('Dotnet Restore') {
      steps {
        script {
          def slnFile = sh(script: 'find . -name "*.sln"', returnStdout: true).trim()
          sh "nuget restore ${slnFile}"
        }
      }
    }

    stage ('Veracode SCA Scan') {
      steps {
        sh 'curl -sSL  https://download.sourceclear.com/ci.sh | sh -s -- scan --url https://github.com/lDivision/NodeGoat'
      }
    }
  }
}
