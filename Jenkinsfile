node{
    stage('Clone') {
        git 'https://github.com/MartinSE6/app-salaire.git'
    }
    stage('Ansible') {
      ansiblePlaybook (
          colorized: true, 
          become: true,             
          playbook: 'playbook.yml',
          inventory: 'hosts.yml'
      )
    }
}
