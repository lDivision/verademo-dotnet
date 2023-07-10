pipeline {
  agent any

  stages {
    stage ('Dotnet Restore') {
      steps {
        script {
          sh 'dotnet restore **/*.sln'
        }
      }
    }
  }
}
