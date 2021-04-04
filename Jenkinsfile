pipeline{
 agent any

 stages{

 stage('terraform init and apply -dev'){
  steps{
   sh label: '', returnStatus: true, script: 'terraform workspace new dev'
   sh "/usr/local/bin/terraform init"
   }
  }
  
   stage('terraform init and apply -prod'){
    steps{
   sh label: '', returnStatus: true, script: 'terraform workspace new prod'
   sh "/usr/local/bin/terraform init"
   }
  }
  
  
 }
}

def 

