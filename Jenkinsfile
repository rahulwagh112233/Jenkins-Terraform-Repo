
node {
    
    stage('git clone') {

        git branch: 'main', url: 'https://github.com/rahulwagh112233/Terraform-Repo.git'
    }
    stage('terafom init') {
        dir('Jenkins'){
        sh 'terraform init'
        }
    }
    stage('terraform plan') {
        dir('Jenkins'){
        sh 'terraform plan'
        }
       
    }
    stage('terraform plan') {
        dir('Jenkins'){
        sh 'terraform apply -auto-approve'
        }
    }
    
}
