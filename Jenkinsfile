pipeline {
	agent any 
	
	stages {
	    stage('Checkout') {
	        steps {
			checkout scm			       
		      }}
		stage('Build') {
	           steps {
			  sh '/home/owaiss/Downloads/apache-maven-3.9.0/bin/mvn install'
	                 }}
		stage('Deployment'){
		   steps {
		sh 'cp target/pipe1.war /home/owaiss/Downloads/apache-tomcat-9.0.79/webapps'
			}}	
}}