pipeline {
    agent any
    stages {
        stage("Clone my app") {
            echo "Project cloning. . ."
            sh "git clone https://github.com/Anudeep221995/jenkins-demo-html-project.git"
            echo "Project cloning successful"
        }
        stage("Deploy my app") {
            echo "Deploying project. . ."
            sh "cd jenkins-demo-html-project; sudo cp index.html /var/www/html/"
        }
    }
}