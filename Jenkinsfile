pipeline { 
      agent {
	      label {
		      label '172.31.11.74'
	      }
	  }
	  stages {
	         stage ('slave1') {
			   steps {
			     
		     sh "yum install httpd -y"
			 sh "service httpd start"
			 sh "cp -r index.html /var/www/html/"
			 sh "chmod -R 777 /var/www/html/index.html"
			 
			   }
			 }
			 
	  }

}
