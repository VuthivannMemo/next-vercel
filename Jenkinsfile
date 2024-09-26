pipeline{
    agent any   

    tools {nodejs "node_v20.11.0"}
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
