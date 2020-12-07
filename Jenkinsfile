
node{
  
    stage('test advance script') {
      bat '''cd C:\\Users\\40010003\\Desktop\\JS-Jasmineminiproject-main\\Jasmine Frame Work
'''
       echo " SERVICE_NAME = 'html report'"
            echo "current build number: ${currentBuild.number}"
            echo "previous build number: ${currentBuild.previousBuild.getNumber()}"
           
            echo 'BRANCH_NAME = htmlreport"'
            //echo env.BUILD_NUMBER

   
        
         
    }
    stage("checkuot")
    {
bat '''cd C:\\Users\\40010003\\Desktop\\JS-Jasmineminiproject-main\\Jasmine Frame Work
npm install
'''

    }
    stage("execution of code")
    {
        bat '''cd C:\\Users\\40010003\\Desktop\\JS-Jasmineminiproject-main\\Jasmine Frame Work\\src
 node Bank.js'''
       // bat 'node Bank.js'
    }
   stage("execution of test code")
    {
        bat '''cd C:\\Users\\40010003\\Desktop\\JS-Jasmineminiproject-main\\Jasmine Frame Work
 npm install jasmine-node'''
       // bat 'node Bank.js'
    }
   stage("execution of code")
    {
        bat '''cd C:\\Users\\40010003\\Desktop\\JS-Jasmineminiproject-main\\Jasmine Frame Work
 jasmine init'''
       // bat 'node Bank.js'
    }
   stage("execution of code")
    {
        bat '''cd C:\\Users\\40010003\\Desktop\\JS-Jasmineminiproject-main\\Jasmine Frame Work\\src
jasmine'''
       // bat 'node Bank.js'
    }
  
  
  
  
    stage("html report")
    {
        publishHTML([allowMissing: false, alwaysLinkToLastBuild: false, keepAll: false, reportDir: 'C:\\Users\\40010003\\Desktop\\JS-Jasmineminiproject-main\\Jasmine Frame Work', reportFiles: 'SpecRunner.html', reportName: 'HTML Report', reportTitles: ''])
    }
 
}
