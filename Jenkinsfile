pipeline {
   agent any
	
   stages {
      stage ('Compile') {
	      
	  steps {
              withMaven(maven : 'mvn_3_5_4') {
	         sh 'mvn clean compile'
	      }
	   }
       }

	stage ('Testing') {
		
	    steps {
	        withMaven(maven : 'mvn_3_5_4') {
		    sh 'mvn test'
	         }
	    }
	}
	stage ('Package') {
	    steps {
	       withMaven(maven : 'maven_3_5_4'){
		    sh 'mvn package'
	       }
	     }
	 }
    }
}

		   
	     
			    
			      
   
