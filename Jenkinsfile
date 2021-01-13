node{
stage('Build and Test') {
    properties([pipelineTriggers([[$class: 'GitHubPushTrigger'], pollSCM('* * * * *')])])
    checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmod
uleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '0a05aad9-0cb8-4403-bddd-124c62fc0439', url: 'https://github.com/rvemulapati/upstream.git']]])
    echo 'Build and Test has been done'
}
