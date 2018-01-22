node {
    def server = Artifactory.server artifactory-dev.buffact.ca

    def uploadSpec = readfile 'files/*'
    
    def buildInfo1 = server.upload spec: uploadSpec
}
