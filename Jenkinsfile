pipeline {
  agent {
    node {
      label 'node1'
    }

  }
  stages {
    stage('git checkout') {
      steps {
        sh 'echo "Hello Rahi"'
        git(url: 'https://github.com/Mikenpatel/Ansible-learning', branch: 'main')
      }
    }

    stage('Ansible-Playbook') {
      environment {
        name = 'Miken'
      }
      steps {
        ansiblePlaybook 'docker.yml'
      }
    }

  }
}