pipeline{
        agent any
        stages{
            stage('Build'){
                steps{
                    sh "maven clean package"
                }
            }
            stage('Deploy'){
                steps{
                    sh "java -jar target/spring-penguins-0.0.1-SNAPSHOT.jar"
                }
            }
        }
}
