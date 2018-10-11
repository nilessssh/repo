#!/usr/bin/groovy
node('master') {
sh 'git config --global http.sslVerify false'
stage("testing ") {
checkout scm
sh """
zip -r roles.zip roles
echo hmmmm
git add *
git commit -m "asdf"
git push
"""
}
}
