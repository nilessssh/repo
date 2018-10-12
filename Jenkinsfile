#!/usr/bin/groovy 
node('master') {
sh 'git config --global http.sslVerify false'
def scmVars
stage("testing ") {
properties([pipelineTriggers([[$class: 'GitHubPushTrigger'], pollSCM('H/1 * * * *')])])
checkout scm
sh """
echo scmVars.GIT_BRANCH
zip -r roles.zip *
echo hmmmm
"""
echo scmVars.GIT_BRANCH
}
}
