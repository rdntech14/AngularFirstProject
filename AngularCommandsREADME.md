
Commands

Steps 

* Install node js
* Install npm
* install angular
* Create new Project
* Download VS code

```
node -v
```
Install npm

```
npm install -g npm@latest
npm -v
```

install angular
```
npm install -g @angular/cli
ng --version
```

create new angular project
```
ng new <projectname>
```

Download VS code
Open project in vs code 
```
code .
```

Open dev server
```
ng serve --open
ng serve -o
```
Pre-reqiuisite to create component from angular cli

```
npm install -g @angular/cli
```

Create new componenet
```
ng generate component component/todo
ng generate component <pathForComponent>/<componentName>

ng g n component/todo

ng g n <componentName> -it -is 
```

Here 
-it for inline template ( no separate .html file will be created)
-is for inline style ( mean no separate .css file will be created)


Create new Service
```
ng generate service <pathForService>/<serviceName>
ng g s service/todo
```

Create new Module
```
ng g m <moduleName>
```
Add Angular Material
```
ng add @angular/material
```
 
 ## Deployment
```
ng build --prod
```


## Dockerize 

Please code in ```Dockerfile```

```
#stage 1 - download node, install npm, and build project
FROM node:latest as nodejs
WORKDIR /app
COPY . .
RUN npm install
RUN npm run build --prod

#stage 2 - run project
FROM nginx:alpine
COPY --from=nodejs /app/dist/OnlineOrder /usr/share/nginx/html
```

# Docker Commands
```
docker build -t onlineorder .
docker images
docker run -p 80:80 onlineorder
```
