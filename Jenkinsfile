#!/usr/bin/groovy 
node('master') {
sh 'git config --global http.sslVerify false'
stage("testing ") {
checkout scm
sh """
branch=`printenv | grep NODE_NAME | awk -F"=" '{print \$2}'`
zip -r \${branch}-`date '+%Y-%m-%d'`.zip *
echo hmmmm
"""
}
}
