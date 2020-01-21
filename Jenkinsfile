pipeline {
    agent { label 'ACI-Container' }  // This will run the below job in 'ACI-Container' label nodes.
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello World"'
                sh '''
                    echo "Multiline shell steps works too" >> Testfile.txt
                    ls -lah
                '''
            }
        }
    }
}
