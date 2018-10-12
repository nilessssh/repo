#!/usr/bin/groovy 
node('master') {
sh 'git config --global http.sslVerify false'
stage("testing ") {
properties([pipelineTriggers([[$class: 'GitHubPushTrigger'], pollSCM('H/1 * * * *')])])
checkout scm
sh """
env.BRANCH_NAME
zip -r roles.zip *
echo hmmmm
"""
}
}
