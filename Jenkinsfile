pipeline {
    agent any

    environment {
        SNOWFLAKE_CREDS = credentials('snowflake-creds')
    }

    stages {
        stage('Deploy to Snowflake') {
            steps {
                bat """
                snowsql -a GY51478 -u ${SNOWFLAKE_CREDS_USR} -p ${SNOWFLAKE_CREDS_PSW} -d test_db -s test_db.public -f init_snowflake.sql
                """
            }
        }
    }
}


















