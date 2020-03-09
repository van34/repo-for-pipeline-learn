pipeline {
  agent any
  stages {
    stage('Git checkout ') {
      steps {
        git(url: 'https://github.com/van34/repo-for-pipeline-learn.git', branch: 'master ')
      }
    }

    stage('Sonar Analyze ') {
      steps {
        withSonarQubeEnv(installationName: 'sonar ', credentialsId: 'sonarsecret')
      }
    }

  }
}