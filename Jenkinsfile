node {
    docker.withServer('tcp://docker-agent:2375', null) {
        docker.image('tomcat').withRun('--name tomcat -p 9090:8080') {
            sh 'until $(curl --output /dev/null --silent --head --fail http://tomcat:9090); do printf \'.\'; sleep 5; done'
        }
    }
}