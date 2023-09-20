pipeline{
    agent{
        node{
            label 'maven'
        }
    }
    stages{
        stage("clone the code"){
        steps{
            git branch : "maven, url: 'https://"
        }
    }
    environment{
        PATH="/opt/apache-maven-3.9.2/bin:$PATH"
    }
    stage("Build "){
        steps{
            sh 'mvn clean deploy'
        }
    }
}
}