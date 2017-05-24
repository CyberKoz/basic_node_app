node {
 git 'https://github.com/cyberkoz/basic_node_app/'
 stage('Token Sleep') {
 			  kubernetes.pod('buildpod').withImage('centos:7').inside {
			    sh 'echo "Hello World!"'
			    sh 'sleep 10'
			  }
 }
}
