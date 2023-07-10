pipeline {
  agent anu

  stages {
    stage ('Dotnet Restore') {
      steps {
        sh 'dotnet restore **/*.sln'
      }
    }
  }


  
}
