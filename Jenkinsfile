#!/usr/bin/groovy
node('master') {
sh 'git config --global http.sslVerify false'
stage("testing ") {
checkout scm
sh """
zip -r role.zip role
echo hmmmm
"""
}
}
