pipeline {
    agent any
    stages {
        stage('Example') {
            steps { 
                echo 'Hello World'
                script{
                    bat'''cd "C:\\Users\\Guangzeng Chen\\Desktop"
                    del *.cpp
                    del *.exe
                    pause
                    cd C:\\Windows\\System32\\config\\systemprofile\\AppData\\Local\\Jenkins.jenkins\\workspace\\pipeline-test
                    dir *.cpp /b >nihao.txt
                    set /p T=<nihao.txt
                    copy %T% C:\\Users\\Guangzeng Chen\\Desktop
                    pause
                    cd "C:\\Users\\Guangzeng Chen\\Desktop"
                    pause
                    g++ -o %T:~0,-4% %T%
                    pause
                    copy %T:~0,-4%.exe C:\\Windows\\System32\\config\\systemprofile\\AppData\\Local\\Jenkins.jenkins\\workspace\\pipeline-test
                    cd C:\\Windows\\System32\\config\\systemprofile\\AppData\\Local\\Jenkins.jenkins\\workspace\\pipeline-test
                    %T:~0,-4%.exe
                    del nihao.txt
                    pause
                    del %T:~0,-4%.exe 
                    pause'''
                }
            }
        }
    }
}

