pipeline{
    agent any 
    stages{
        stage ('compile stage'){
            
            steps{
                withMaven (maven : 'maven'){
                    sh 'mvn clean compile'
                }
            }
        }
        stage ('Test stage'){
            
            steps{
                withMaven (maven : 'maven'){
                    sh 'mvn test'
                }
            }
        }
        stage ('Deploy stage'){
            
            steps{
                withMaven (maven : 'maven'){
                    sh 'mvn deploy'
                }
            }
        }    
}
}
