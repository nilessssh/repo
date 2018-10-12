#!/usr/bin/groovy 
node('master') {
sh 'git config --global http.sslVerify false'
stage("testing ") {
checkout scm
sh """
printenv | grep NODE_NAME
zip -r roles.zip *
echo hmmmm
"""
}
}
