podTemplate(cloud:'minikube', label: 'buildpod', containers: [
    containerTemplate(name: 'jnlp', image: 'jenkinsci/jnlp-slave:2.62-alpine', args: '${computer.jnlpmac} ${computer.name}'),
    containerTemplate(name: 'centos', image: 'centos:7', ttyEnabled: true, command: '/usr/bin/cat')
]) {
    node('buildpod') {
        stage('Run shell') {
            container('centos') {
                sh 'echo "hello world!!!"'
            }
        }
    }
}
