Test setup for running docker containers on a remote docker agent (docker-agent) from Jenkins (ci).

Steps:
1. docker-compose up, starts the docker-agent and ci containers
2. Complete Jenkins installation
3. Create a pipeline job on Jenkins that uses the Jenkinsfile in this repo
