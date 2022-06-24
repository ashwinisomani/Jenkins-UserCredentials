
CRUMB=`curl -u $asomani:$Freebird$29 'http://localhost:8080/crumbIssuer/api/xml?xpath=concat(//crumbRequestField,":",//crumb)'`
curl -H $CRUMB -X POST http://localhost:8080/job/AutomatedUserCreation/buildWithParameters?token=<myToken> -F email=abc@edifecs.com
  
  verbosity=high

json={
  ":" "0",
  "credentials": {
    "scope" : "'{{GLOBAL}}'"
    "id" : "'{{ii.ssh_user}}'"
    "username" : "'{{ii.ssh_user}}'"
    "password" : ""
    "description" : "'{{ii.ssh_user}}'"
    "stapler-class" : "'{{com.cloudbees.jenkins.plugins.sshcredentials.impl.BasicSSHUserPrivateKey}}'"
  }
}
