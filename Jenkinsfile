pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
              
                // Get some code from a GitHub repository
                //git 'https://github.com/jglick/simple-maven-project-with-tests.git'

                // Run Maven on a Unix agent.
                //mvnHome = '/usr/local/apache-maven-3.9.8'
                //sh "mvn -Dmaven.test.failure.ignore=true clean package"

                // To run Maven on a Windows agent, use
                //sh '"$MVN_HOME/bin/mvn" -Dmaven.test.failure.ignore clean package'
                sh '"/usr/local/apache-maven-3.9.8/bin/mvn" -Dmaven.test.failure.ignore clean package'
            }

        }
    }
}
