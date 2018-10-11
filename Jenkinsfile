#!/usr/bin/groovy
node('master') {
sh 'git config --global http.sslVerify false'
stage("testing ") {
checkout scm
sh """
sudo ip -r roles.zip roles
echo hmmmm
"""
}
}
