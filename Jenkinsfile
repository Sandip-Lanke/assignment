pipeline { 
      agent { 
		      label 'built-in'
	      
	  }
	  stages {
	         stage ('master') {
			   steps {	     
		     sh"yum install httpd -y"
			 sh "sudo service httpd start"
			 sh "sudo cp -r index.html /var/www/html/"
			 sh "sudo chmod -R 777 /var/www/html/index.html"
			 
			   }
			 }
			 
	  }

}
