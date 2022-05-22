

<img src="https://th.bing.com/th/id/Rdf9c581c44ea9940d1f60d5cc4bc1752?rik=rLnrGxQ5XA8Uzg&pid=ImgRaw" width="100"><img src="https://www.ictdemy.com/images/5728/nodejs_logo.png" width="80">
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d2/Oauth_logo.svg/1920px-Oauth_logo.svg.png" width="90">




# k8s-clean-arch-typescript-microservice
Clean architecture microservices in typescript and deployment In kubernetes.



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
