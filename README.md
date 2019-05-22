# jenkins

aktuelles image ziehen:

	docker pull jenkinsci/blueocean

und starten

	docker run -p 8080:8080 jenkinsci/blueocean

bzw.

	docker stack deploy -c docker-compose.yml myjenkins
  
 
