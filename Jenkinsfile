pipeline {
     agent any
     stages {
        stage("Build") {
            steps {
                sh "sudo npm install"
                sh "sudo npm run build"
            }
        }
		
        stage("Deploy") {
            steps {
                sh "sudo rm -rf ~/workspace/jenkins-react-app1"
                sh "sudo cp -r ~/workspace/jenkins-react-app1/"
            }
        }
    }
}