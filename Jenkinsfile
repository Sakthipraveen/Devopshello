pipeline {
    agent any
    environment{
		PATH= "E:\devops\Maven\apache-maven-3.8.1\bin:$PATH"
	
	}

    stages {
        stage('Git Integration') {
            steps {
                git url: 'https://github.com/Sakthipraveen/Devopshello'
            }
        }
		
        stage('Maven') {
            steps {
                sh "mvn clean install package"
            }
        }
    }
}
