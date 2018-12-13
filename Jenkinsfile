pipeline{
   agent any
       stages{
         stage('compile'){
	               steps{
                          withMaven(maven : 'maven_3_5_3'){
			      sh 'mvn clean compile'
			      }
			      }
			      }

	stage('testing'){
	          steps{
		      withMaven(maven : 'maven_3_5-3'){
		             sh 'mvn mvn test'
			     }
			     }
			     }
	stage('package'){
	         steps{
		    withMaven(maven : 'maven_3_5_3'){
		            sh 'mvn package'
			    }
			    }
			    }
	 }
	 }

		   
	     
			    
			      
   
