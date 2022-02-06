# nginx-docker-deployment
deploying any production grade application using nginx in docker container


### Apply the local changes in runtime :
	
	$ pwd

	$ docker run -p 8080:80 -v $(pwd):/usr/share/nginx/html myweb 

### docker files
"Dockerfile"  -> final wrapper (production based)
.dockerignore -> avoids files/folder from pushing into prod
Docker-compose.yml -> replacement for writing in command (keep code in this instead of command line)
Dockerfile.dev -> specifically for development / testing (staging)