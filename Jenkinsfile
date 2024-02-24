pipeline {
	agent any 
	
	stages {
	    stage('Checkout') {
	        steps {
			checkout scm			       
		      }}
		stage('Build') {
	           steps {
			  sh '/home/lina/Documents/extract_tar_files/apache-maven-3.9.6/bin/mvn install'
	                 }}
		stage('Deployment'){
		   steps {
		sh 'cp target/pipeline.war /home/lina/Documents/extract_tar_files/apache-tomcat-9.0.85/webapps'
			}}	
}}
