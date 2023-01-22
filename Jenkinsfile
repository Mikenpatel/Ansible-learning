pipeline {
  agent any
  stages {
    stage('git checkout') {
      steps {
        sh 'echo "Hello Rahi"'
        git(url: 'https://github.com/Mikenpatel/Ansible-learning', branch: 'main')
      }
    }

    stage('Ansible-Playbook') {
      steps {
        ansiblePlaybook 'docker.yml'
      }
    }

  }
}