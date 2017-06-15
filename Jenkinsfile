node() {
   
stage ('Build') {

    git url: 'https://github.com/rakshitha2/test_proj.git'

    def mvnHome = tool 'M3'
  echo 'about to change dir'

  dir ('tibco.bw.sample.binding.soap.http.BookStore.application.parent') {
 pwd()
 bat "${mvnHome}\\bin\\mvn install"
}
  echo 'changed dir'
  
}
stage ('push_jenkinsfile') {

     bat("git config --global http.proxy http://rakshitha.a:Welcome27@blr-sezproxy.hcl.com:8080)
     bat("git config --global https.proxy http://rakshitha.a:Welcome27@blr-sezproxy.hcl.com:8080)
     bat("git tag -a some_tag1 -m 'Jenkins'") 
     bat('git push https://${rakshitha2}:${devops2017}@https://github.com/rakshitha2/test_proj.git') 
}
}