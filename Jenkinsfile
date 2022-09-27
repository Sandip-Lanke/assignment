pipeline { 
      agent {
	      label {
		      label '172.31.11.74'
	      }
	  }
	  stages {
	         stage ('slave1') {
			   steps {
			 sh "sudo rm -rf *"
			sh "sudo yum install git -y"	   
		         sh"sudo yum install httpd -y"
			 sh "sudo service httpd start"
			 sh "sudo cp -r index.html /var/www/html/"
			 sh "sudo chmod -R 777 /var/www/html/index.html"
			 
			   }
			 }
			 
	  }

}
