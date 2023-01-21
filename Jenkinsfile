pipeline {  
    agent any  
        stages {  
       	    stage("git_checkout") {  
           	    steps {  
              	    echo "cloning repository" 
              	    echo "repo cloned successfully"  
              	    }  
         	    }
		    stage('Build') {
            steps {
                dir("/var/lib/jenkins/workspace/store/") {
                sh 'mvn -B -DskipTests clean package'
				sh 'built done'
                }
            } 
        }
}
}
