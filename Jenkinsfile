
node{
  
    stage('test advance script') {
       echo " SERVICE_NAME = 'html report'"
            echo "current build number: ${currentBuild.number}"
            echo "previous build number: ${currentBuild.previousBuild.getNumber()}"
           
            echo 'BRANCH_NAME = Jasmine Frame Work"'
      echo env.BUILD_NUMBER
 def  Latest_Build_Number = env.BUILD_NUMBER
      echo 'TAG = "${BRANCH_NAME}_$value: env.BUILD_NUMBER}"'
        
         
    }
    stage("checkuot")
    {
bat '''cd C:\\Users\\40010003\\Desktop\\JS-Jasmineminiproject-main\\Jasmine Frame Work\\spec 
npm install
'''

    }
    stage("execution of code")
    {
        bat '''cd C:\\Users\\40010003\\Desktop\\JS-Jasmineminiproject-main\\Jasmine Frame Work\\src
 node Bank.js'''
       // bat 'node Bank.js'
    }
    stage("html report")
    {
        publishHTML([allowMissing: false, alwaysLinkToLastBuild: false, keepAll: false, reportDir: 'C:\\Users\\40010003\\Desktop\\JS-Jasmineminiproject-main\\Jasmine Frame Work', reportFiles: 'SpecRunner.html', reportName: 'HTML Report', reportTitles: ''])
    }
 
}
