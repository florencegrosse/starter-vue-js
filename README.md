# Starter Front : project.DMN.io

> Starter with VueJS, VueX, Vue-ROUTER, Vue-RESOURCE, Capistrano...

> quentin.tshaimanga@edf.fr

## Build Setup
### install dependencies localy
```
npm install
```

## Dev
### serve with hot reload at localhost:8080
```shell
npm run dev
```

## Build and Production in project.DMN.io
```
  - [server] create /var/www/projectName/
  - set deploy.rb : repo and name
```
```
  - After git add / commit / push
  - cap production deploy (set server info before automatic install and build)
  - cap production apache:conf (set apache conf)
  - cap production apache:ssl (set ssl_file conf)
```
````
  - set or renew TLS certificat : /opt/letsencrypt/letsencrypt-auto
````

### App crash > rollbask to the previous release
```shell
cap production deploy:rollback
```

## Prod
```shell
npm run build
```
