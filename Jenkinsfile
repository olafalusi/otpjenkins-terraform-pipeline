pipeline{
  agent any
  environment {
    PATH = "${PATH}:${getTerraformPath()}"
}
  stages{
    stage('terraform init'){
      steps{
        sh "terrform init"
      }
    }
  }
}

def getTerraformPath(){
  def tfHome = tool name: 'Terraform-12', type: 'org.jenkinsci.plugins.terraform.TerraformInstallation
  return tfHome
