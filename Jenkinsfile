
pipeline {
    agent {node {label "Slave1"}}
    environment {
    NEW_VERSION = '1.3.0'
    }
    
    stages {
        stage("build"){
            steps {
            echo "This is Build stage"
            echo "Branch_name" +env.BRANCH_NAME  
            echo "Node Name :- "+env.NODE_NAME 
            echo "Building version :- ${NEW_VERSION}"   
            echo 'Building version :- ${NEW_VERSION}'
}
            
        }
        stage("test"){
            when {
                expression {
                env.BRANCH_NAME="main" 
                }
            }
            steps {
            echo "This is test stage"
 }
            
        }
        stage("deploy"){
            steps {
            echo "This is deploy"
}
            
        }
        stage("monitor"){
            steps {
            echo "This is monitor"
               
}
            
        }
    }
    post {
        always{echo "I am always in post action"}
        success{echo "I am success in post action"}
        failure{echo "I am failure in post action"}
    }   
}
