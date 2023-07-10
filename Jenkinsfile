pipeline {
  agent any

  stages {
    stage ('Dotnet Restore') {
      steps {
        sh 'dotnet restore **/*.sln'
      }
    }
  }


  
}
