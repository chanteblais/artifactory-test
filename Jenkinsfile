def server = Artifactory.server "Artifactory-Dev"
def uploadSpec

node (label: 'jbuild01_docker') {
    def app

    stage('Clone repository') {

        checkout scm
    }
    
    stage('Upload') {
        
        uploadSpec = """{
          "files": [
            {
              "pattern": "artifactory-test-master/files/",
              "target": "my-repository"
            }
         ]
        }""" 
        
        server.upload(uploadSpec)
    }
}
