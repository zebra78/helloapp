pipeline {

    agent any

    stages {
        stage('Clone support repos') {
            steps {
                dir('env') {
                    git branch: 'tst', credentialsId: 'jenkins_gitbucket', url: 'ssh://git@192.168.100.100:29418/hello/helloenv.git'
                }
                dir('cfm') {
                    git branch: 'tst', credentialsId: 'jenkins_gitbucket', url: 'ssh://git@192.168.100.100:29418/hello/hellocfm.git'
                }
            }
        }
    }

}
