node {
    def server = Artifactory.server 'artifact01'

    def uploadSpec = readfile 'files/*'
    
    def buildInfo1 = server.upload spec: uploadSpec
}
