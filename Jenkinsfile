node{
 stage('Clone') {
   git 'https://github.com/MartinSE6/app-salaire.git'
 }
 stage('Ansible') {
    ansiblePlaybook (
    colorized: true, 
    become: true, 
    playbook: 'install_table.yaml',
    inventory: 'inventaire',
    disableHostKeyChecking: true
    )
  }
}
