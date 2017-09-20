parallel windowsBuild: {
  node () {
    stage('Clean Up Workspace - Windows') {
      step([$class: 'WsCleanup'])
    }

    stage('Prepare Environment - Windows') {
      println 'Preparing Windows environment'
    }

    stage('Install Dependencies - Windows') {
      println 'Installing dependencies on Windows'
    }
          
    stage('Lint Project - Windows') {
      println 'Linting project on Windows'
    }

    stage('Run Unit Tests - Windows') {
      println 'Running unit tests on Windows'
    }

    stage('Build - Windows') {
      println 'Building on Windows'
    }

    stage('Publish App - Windows') {
      println 'Publishing app for Windows'
    }

  }

}, macBuild: {
  node () {
    stage('Clean Up Workspace - Mac') {
      step([$class: 'WsCleanup'])
    }

    stage('Prepare Environment - Mac') {
      println 'Preparing Mac environment'
    }

    stage('Install Dependencies - Mac') {
      println 'Installing dependencies on Mac'
    }
          
    stage('Lint Project - Mac') {
      println 'Linting project on Mac'
    }

    stage('Run Unit Tests - Mac') {
      println 'Running unit tests on Mac'
    }

    stage('Build - Mac') {
      println 'Building on Mac'
    }

    stage('Publish App - Mac') {
      println 'Publishing app for Mac'
    }

  }

}, failFast: false

stage('Prompt for Production Deploy') {
  timeout(time: 2, unit: 'DAYS') {
    input message: 'Deploy to Production?'
  }
}

node() {
  stage('Deploy Installer to Production') {
    println 'Deploying to Production'
  }
}

