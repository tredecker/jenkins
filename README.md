# Jenkins

aktuelles image ziehen:

	docker pull jenkinsci/blueocean

und starten

	docker run -d -p 8080:8080 jenkinsci/blueocean

bzw.

	docker stack deploy -c docker-compose.yml myjenkins

to get container ID

	docker container ls

to get initialAdminPassword

	docker logs <container ID>

visit http://localhost:8080 and paste initialAdminPassword
then install plug-ins



