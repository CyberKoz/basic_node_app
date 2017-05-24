kubernetes.pod('buildpod').withNewContainer().withName('centos').withImage('centos:6').inside {
    git 'https://github.com/cyberkoz/basic_node_app/'
	sh 'sleep 10'
}
