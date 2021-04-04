pipeline{
 agent any

environment {
 PATH = "${PATH}:${TerraformPath()}"
}
 stages{

 stage('terraform init'){
  steps{
   sh "terraform init"
   }
  }
 }
}

def get TerraformPath(){
 def tfHome = tool name: 'terraform-12', type: 'org.jenkinsci.plugins.terraform.TerraformInstallation'
 return tfHome
}
