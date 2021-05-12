pipeline {
    agent {node {label "Slave1"}}
    
    stages {
        stage("Build project1"){
            steps {
            echo "This is Build project1"
            build project1}
            
        }
        stage("Build Project2"){
            steps {
            echo "This is Build project2"
            build project2 }
            
        }
        stage("Build project3"){
            steps {
            echo "This is Build project3"
            build project3 }
            
        }
        stage("Build Project3"){
            steps {
            echo "This is Build project4"
            build project4 }
            
        }
    }
}
