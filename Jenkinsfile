#!/usr/bin/groovy 
node('master') {
sh 'git config --global http.sslVerify false'
stage("testing ") {
checkout scm
sh """
branch=`printenv | grep NODE_NAME | awk -F"=" '{print \$2}'`
zip=`zip -r \${branch}-`date '+%Y-%m-%d'`.zip *`
cp \${zip} \${zip}.new
echo hmmmm
"""
}
}
