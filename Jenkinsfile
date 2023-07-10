pipeline {
  agent {
    docker {image 'ldivision/ubuntu:latest'}
  }

  stages {
    stage ('Dotnet Restore') {
      steps {
        sh 'dotnet restore **/*.sln'
      }
    }
  }


  
}
