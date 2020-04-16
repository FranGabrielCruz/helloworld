pipeline{
    agent any
    tools {
        maven 'Maven_3.5.2' 
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
