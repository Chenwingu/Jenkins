pipeline {
    
    agent any
    
    parameters {
        booleanParam(name: "RELEASE", defaultValue: false)
    }
    
    stages {

        stage("Build") {
            steps {
                echo "build war file"
            }
        }
        
        stage("Publish") {
            when { expression { params.RELEASE } }
            steps {
               echo "Deploying ..."
            }
        }
    }
}
