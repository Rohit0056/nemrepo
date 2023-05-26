pipeline {
  agent any
  stages {
    stage('FETCH from SCM/GITHUB') {
      steps {
        git(url: 'https://github.com/Rohit0056/nemrepo.git', branch: 'main', poll: true, credentialsId: 'Rohit0056')
      }
    }

    stage('Install APACHE') {
      steps {
        sh '''sudo apt install apache2 -y
'''
      }
    }

    stage('DEPLOYMENT') {
      steps {
        sh 'sudo cp -R * /var/www/html'
      }
    }

  }
}