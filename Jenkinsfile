job {
  name 'Build'
  scm {
      git('https://github.com/cyberkoz/basic_node_app/')
  }
  steps {
  		podTemplate(label: 'nodejs', containers: [
				   containerTemplate(name: 'centos', image: 'centos:6', ttyEnabled: true, command: '/bin/bash')
		]) {
		   node('nodejs') {
               stage('Run shell') {
                   sh 'sleep 10'
        	   }
    	   }
		}
	}
}
