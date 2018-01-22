node {
    def server = Artifactory.server 'artifact01'

    def uploadSpec = """{
        "files": [
          {
            "pattern": "files/file1",
            "target": "my-repository/test/"
          }
        ]
      }"""
    
    server.upload (uploadSpec)
}
