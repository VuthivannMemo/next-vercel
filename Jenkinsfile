pipeline{
    agent any   

    tools {nodejs "node"}
    stages{
        stage("Install dependencies"){
            steps{
                bat 'npm install'
                echo "Install dependencies successfully"
            }
        }
        stage("Build"){
            steps{
                bat 'npm run build'
                echo "App built successfully"
            }
        }
    }
}
