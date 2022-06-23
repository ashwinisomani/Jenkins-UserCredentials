  curl  http://localhost:8080/job/AutomatedUserCreation/buildWithParameters?token=<myToken> -F email=abc@edifecs.com
  verbosity=high

json={
  ":" "0",
  "credentials": {
    "scope" = "'{{GLOBAL}}'"
    "id" = "'{{ii.ssh_user}}'",
    "username" = "'{{ii.ssh_user}}'",
    "password" = "",
    "privateKeySource" = {
      "stapler-class": "com.cloudbees.jenkins.plugins.sshcredentials.impl.BasicSSHUserPrivateKey$FileOnMasterPrivateKeySource",
      "privateKeyFile": "'{{jenkins_home}}/{{ii.key_name}}.pem'",
    },
    "description" = "'{{ii.ssh_user}}'",
    "stapler-class" = "com.cloudbees.jenkins.plugins.sshcredentials.impl.BasicSSHUserPrivateKey"
  }
}
