pipeline {
  agent any
    environment {
      PATH='C:/Program Files/Git/bin/git.exe'
    }

  stages {

    stage('NPM Setup') {
      steps {
          sh 'npm install'
      }
    }

    stage('Android Build') {
      steps {
          sh 'ionic cordova build android'
      }
    }

    // stage('APK Sign') {
    //   steps {
    //     sh 'jarsigner -storepass your_password -keystore keys/yourkey.keystore platforms/android/app/build/outputs/apk/release/app-release-unsigned.apk nameApp'
    //   }
    // }

    stage('Publish Android') {
      steps {
        echo "Publish Android API Action"
      }
    }

  }
}
