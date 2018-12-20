pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running build automation'
                sh './gradle build --no-daemon'
                archiveArtifacts artifacts: 'build/lib/gradle-java-ear.ear'
            }
        }
    }
}
