# DockerConfig
Docker configuration of home server to learn about containers and server setups

## Installation  
- make sure both docker and docker-compose are installed
- pull the repo 
- create a folder `Volumes` alongside the repo
- add a `user-SHA1(pwd)`pair into `<current-dir>/Volumes/traefik/basic-auth-userfiles/traefik-dashboard`
- if required change names & domains (+ configure DNS)
- start up traefik  `docker-compose -f docker-compose-traefik.yml up -d` 
- verify everything works as expected (browse to the dashboard and login with the password you put in the file)


## Documentation
### Traefik
- [v2.2 documentation](https://docs.traefik.io/user-guides/docker-compose/acme-tls/)
- [understanding + additions to docs](https://containo.us/blog/traefik-2-0-docker-101-fc2893944b9d/)
- [same but different](https://blog.creekorful.com/how-to-expose-traefik-2-dashboard-securely-docker-swarm/)
