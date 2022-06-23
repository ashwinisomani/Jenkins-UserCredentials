CRUMB=$(curl -s 'http://user:token@jenkins_server:8080/crumbIssuer/api/xml?xpath=concat(//crumbRequestField,":",//crumb)')
curl -H $CRUMB -X POST 'http://user:token@jenkins_server:8080/credentials/store/system/domain/_/createCredentials' \
--data-urlencode 'json={
  "": "0",
  "credentials": {
    "scope": "GLOBAL",
    "id": "identification",
    "username": "manu",
    "password": "bar",
    "description": "linda",
    "$class": "com.cloudbees.plugins.credentials.impl.UsernamePasswordCredentialsImpl"
  }
}'
