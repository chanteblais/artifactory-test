pipeline {
    agent { 
        label 'SlaveNode' 
    }
    stages {
        stage('download') {
            def server = Artifactory.server "artifact01"
            def downloadSpec = """{
                "files": [
                  {
                      "pattern": my-repository/test/,
                      "target": "bazinga/"
                    }
                ]
            }"""   
        }
    }
}
