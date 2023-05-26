pipeline {
  agent any
  stages {
    stage('Fetch from SCM') {
      parallel {
        stage('Fetch from SCM') {
          steps {
            git(url: 'https://github.com/Rohit0056/nemrepo.git', branch: 'main', credentialsId: 'Rohit0056', poll: true)
          }
        }

        stage('') {
          steps {
            git(url: 'https://github.com/Rohit0056/nemrepo.git', branch: 'main', poll: true, credentialsId: 'Rohit0056')
          }
        }

      }
    }

  }
}