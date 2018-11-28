node{
  stage ('Checkout')
  {
      git credentialsId: 'dd857b59-e8e0-4ef2-928b-952e499489ee', url: 'https://github.com/shriyanshbansal/Node-Web-App.git'
  }
  
  stage('Run the Playbook'){
    ansiblePlaybook disableHostKeyChecking: true, extras: 'action=$action server=$server', inventory: 'hosts', playbook: 'main.yml'

  }
}
