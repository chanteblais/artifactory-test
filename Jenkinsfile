node {
    def server = Artifactory.server SERVER_ID

    def uploadSpec = readfile 'files/*'
    
    def buildInfo1 = server.upload spec: uploadSpec
}
