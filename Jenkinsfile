pipeline {
  agent {
    docker {
      image 'node:20-alpine'
    }

  }
  stages {
    stage('install dependencies') {
      steps {
        sh 'npm install'
      }
    }

    stage('build') {
      steps {
        sh '$ npm run build'
      }
    }

  }
  environment {
    REACT_APP_GEMINI_API_KEY = 'AIzaSyDjsJlhW6ls16eS57PeGGJKq7GPlPfjzNY'
  }
}
