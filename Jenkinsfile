#!/usr/bin/groovy 
node('master') {
sh 'git config --global http.sslVerify false'
stage("testing ") {
checkout scm
sh """
branch=`printenv | grep NODE_NAME | awk -F"=" '{print \$2}'`
zip -r \${branch}-`date '+%Y-%m-%d'`.zip *
cp \${branch}-`date '+%Y-%m-%d'`.zip \${branch}-`date '+%Y-%m-%d'`.zip.zip
echo hmmmm
"""
}
}
