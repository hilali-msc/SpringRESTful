pipeline {
    agent any
    tools {maven "MH-maven"}
    stages {
        stage("checkout") {
            steps {
                git branch: "main", url: "https://github.com/hilali-msc/SpringRESTful.git"
            }
        }
        stage("build") {
            steps {
               sh "mvn compile"
            }
        }
        stage("test") {
            steps {
                sh "mvn test"
            }
        }        
    }
}
