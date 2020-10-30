

node {

    stage('Initialize'){       
        def mavenHome  = tool 'myMaven'
        //env.PATH = "${dockerHome}/bin:${mavenHome}/bin:${env.PATH}"
	    env.PATH = "${mavenHome}/bin:${env.PATH}"
    }

    stage('Checkout') {
        checkout scm
    }

    stage('Build'){
        sh "mvn clean install"
    }


}






