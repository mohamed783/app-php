node{
 stage('Clone') {
   git 'https://github.com/MartinSE6/app-salaire.git'
 }
 stage('Ansible') {
    ansiblePlaybook (
    colorized: true, 
    playbook: 'playbook.yaml',
    inventory: 'inventaire',
    )
  }
}
