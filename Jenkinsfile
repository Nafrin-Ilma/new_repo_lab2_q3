pipeline {
  agent any

  tools {
    // Install the Maven version configured as "M3" and add it to the path.
    maven "maven3"
  }

  stages {
    stage('Build') {
      steps {
        // Get some code from a GitHub repository
        git branch: 'main', url: 'https://github.com/Nafrin-Ilma/new_repo_lab2_q3'
      }
    }
    stage('Compile') {
      steps {
        bat 'mvn clean compile'
      }
    }
  }
}
