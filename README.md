# Jenkins

aktuelles image ziehen:

	docker pull jenkinsci/blueocean

und starten

	docker run -d -p 8080:8080 jenkinsci/blueocean
	docker run -d -p 8080:8080 -p 50000:50000 -v /var/run/docker.sock:/var/run/docker.sock -v /Users/tom/Documents/Jenkins:/var/jenkins_home jenkinsci/blueocean

bzw.

	docker stack deploy -c docker-compose.yml myjenkins

to get container ID

	docker container ls

to get initialAdminPassword

	docker logs <container ID>

visit http://localhost:8080 and paste initialAdminPassword
then install suggested plug-ins



