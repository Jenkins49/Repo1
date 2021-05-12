CODE_CHANGES = getGitChanges()
pipeline {
    agent {node {label "Slave1"}}
    
    stages {
        stage("build"){
            when {
                expression {
                BRANCH_NAME="dev" || CODE_CHANGES=true
                }
            }
            steps {
            echo "This is Build stage"
}
            
        }
        stage("test"){
            when {
                expression {
                BRANCH_NAME="main" || BRANCH_NAME="dev"
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
