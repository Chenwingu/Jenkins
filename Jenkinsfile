pipeline {
  agent any
  
  parameters {
    booleanParam(name: "RELEASE", defaultValue: false)
    
  }
  
  stages {
    stage("build")
    {
      steps {
        echo "build the code"
      }
    }
    
    stage("Publish") {
      when { expression { params.RELEASE} }
      steps{
        echo "Release code to next environment"
      }
    }
  }
}
