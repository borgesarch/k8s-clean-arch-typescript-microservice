<img src="https://kubernetes.io/images/nav_logo.svg" width="300">
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/7/7e/Node.js_logo_2015.svg/1280px-Node.js_logo_2015.svg.png" width="200">

# k8s-clean-arch-typescript-microservice
Clean architecture typescript and deployment In kubernetes.



# #

[![License](https://img.shields.io/badge/License-MIT-silver.svg?style=flat)](https://github.com/clips/pattern/blob/master/LICENSE.txt) 
[![License](https://img.shields.io/badge/Node-14.17.0.LTS-green.svg?style=flat)](https://github.com/clips/pattern/blob/master/LICENSE.txt) 
[![License](https://img.shields.io/badge/KeyCloak-13.3.1-silver.svg?style=flat)](https://github.com/clips/pattern/blob/master/LICENSE.txt) 
[![License](https://img.shields.io/badge/Kubernetes-1.20.2-blue.svg?style=flat)](https://github.com/clips/pattern/blob/master/LICENSE.txt) 

##


Deployment in one command
```sh
$ bash deploy.sh
```


SSO Authorization:

```sh

curl --request POST \
  --url {{url}}/auth/realms/{{CLOAK_RELM}}/protocol/openid-connect/token \
  --header 'Content-Type: application/x-www-form-urlencoded' \
  --data grant_type=password \
  --data client_id={{CLIENT_ID}} \
  --data client_secret={{CLIENT_SECRET}} \
  --data username={{USERNAME}} \
  --data password=={{PASSWORD}}

```


Testing using sso on micro-service:

```sh
curl --request GET \
  --url {{url}}/users
```
