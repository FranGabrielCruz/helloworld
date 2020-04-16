pipeline{
    agent any
    tools {
        maven 'maven' 
    }
    stages{
        stage('Build'){
            steps{
                withMaven(
                maven: 'maven-3',
                    mavenSettingsConfig: 'my-maven-settings'
                ){
                sh 'mvn clean package'
                }
            }
        }
    }
}
