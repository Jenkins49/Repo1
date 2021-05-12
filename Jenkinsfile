pipeline {
    agent {node {label "Slave1"}}
    
    stages {
        stage("Build project1"){
            steps {
            echo "This is Build project1"
}
            
        }
        stage("Build Project2"){
            steps {
            echo "This is Build project2"
 }
            
        }
        stage("Build project3"){
            steps {
            echo "This is Build project3"
}
            
        }
        stage("Build Project3"){
            steps {
            echo "This is Build project4"
                build job1
}
            
        }
    }
    post {
        always{echo "I am always in post action"}
        success{echo "I am success in post action"}
        failure{echo "I am failure in post action"}
    }   
}
