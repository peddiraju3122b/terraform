pipeline{
    agent{label 'jdk11'}
    stages{
        stage ('terraform'){
            steps(clone){
                git url: 'https://github.com/peddiraju3122b/terraform.git',
                branch: 'main'                
            }
            }
        
        stage ('terraforminit'){
             steps{
                sh 'terraform init'
                sh 'terraform apply -auto-approve'
                }
            }
    }
}
