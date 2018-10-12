#!/usr/bin/groovy 
node('master') {
sh 'git config --global http.sslVerify false'
stage("testing ") {
checkout scm
sh """
printenv | grep NODE_NAME | awk -F"=" '{print $2}'
zip -r roles.zip *
echo hmmmm
"""
}
}
