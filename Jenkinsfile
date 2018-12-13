pipeline{
   agent any
	
   stages {
      stage ('Compile') {
	      
	  steps {
             withMaven(maven : 'maven_3_5_3') {
	         sh 'mvn clean compile'
		 }
	   }
       }

	stage('Testing'){
	          steps{
		      withMaven(maven : 'maven_3_5_3'){
		             sh 'mvn test'
			     }
			     }
			     }
	stage('Package'){
	         steps{
		    withMaven(maven : 'maven_3_5_3'){
		            sh 'mvn package'
			    }
			    }
			    }
	 }
	 }

		   
	     
			    
			      
   
