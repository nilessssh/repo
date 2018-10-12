#!/usr/bin/groovy 
def scmVars
node('master') {
sh 'git config --global http.sslVerify false'
stage("testing ") {
checkout scm
sh """
zip -r roles.zip *
echo hmmmm
"""
}
stage("zip") {
echo scmVars.GIT_BRANCH
}
}
