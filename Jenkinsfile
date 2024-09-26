pipeline{
    agent any    
    stages{
        stage("checkout") {
            steps{
                checkout scm
            }
        }
        stage("Install NPM") {
            steps{
                sh 'sudo apt install npm'
                echo "Install npm successfully"
            }
        }
        stage("Install dependencies"){
            steps{
                sh 'npm install'
                echo "Install dependencies successfully"
            }
        }
        stage("Build"){
            steps{
                sh 'npm run build'
                echo "App built successfully"
            }
        }
    }
}
