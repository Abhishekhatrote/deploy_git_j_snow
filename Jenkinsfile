



pipeline {
    agent any

    stages {
        stage('Deploy to Snowflake') {
            steps {
                bat '''
                snowsql -a GY51478 -u SURAJ9291 -p SurajHatrote@9291 -d test_db -s test_db.public -f init_snowflake.sql
                '''
            }
        }
    }
}

















