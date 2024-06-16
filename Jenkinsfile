pipeline {
    agent any
    stages {
        stage("Clone my app") {
            steps {
                echo "Project cloning. . ."
                sh "rm -rf jenkins-demo-html-project; git clone https://github.com/Anudeep221995/jenkins-demo-html-project.git"
                echo "Project cloning successful"
            }
           
        }
        stage("Deploy my app") {
            steps {
                echo "Deploying project. . ."
                sh "cd jenkins-demo-html-project; cp index.html /var/www/html/"
            }
           
        }
        stage("Testing my app") {
            steps {
                echo "Testing project. . ."
                sh "curl http://localhost:8080/"
            }
           
        }
    }
}