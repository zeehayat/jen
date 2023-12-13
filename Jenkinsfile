pipeline{
    agent any
    environment{
        staging_server='zeenux.online'
    }
    stages{
        stage('Deploy to Server'){
            steps{
                bat 'scp ${WORKSPACE}/* zeenux@zeenux.online:/home/zeenux/public_html/'
            }
        }
    }
}