pipeline {
    agent {node {label "Slave1"}}
    
    stages {
        stage("build"){
            steps {
            echo "This is Build stage"
}
            
        }
        stage("test"){
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
