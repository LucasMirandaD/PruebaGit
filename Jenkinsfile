pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                git 'https://github.com/LucasMirandaD/PruebaJenkins.git'
                sh 'mvn clean compile'
            }
        }
        
    }
}