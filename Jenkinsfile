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
      
      steps{
        
        script{
          
          if (params.RELEASE) {
            
        echo "Release code to next environment"
      }
      else
      {
        echo " Pre release activites conducted"
      }
    }
  }
}
