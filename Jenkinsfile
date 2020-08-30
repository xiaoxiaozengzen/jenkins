pipeline {
    agent any
    stages {
        stage('Example') {
            steps { 
                echo 'Hello World'
                script{
                    bat"'cd C:\Users\GW00204700\Desktop
del *.cpp
del *.exe
pause
cd C:\Windows\System32\config\systemprofile\AppData\Local\Jenkins.jenkins\workspace\jenkins-git
dir *.cpp /b >nihao.txt
pause
set /p T=<nihao.txt
copy %T% C:\Users\GW00204700\Desktop
pause
cd C:\Users\GW00204700\Desktop
pause
g++ -o %T:~0,-4% %T%
pause
copy %T:~0,-4%.exe C:\Windows\System32\config\systemprofile\AppData\Local\Jenkins.jenkins\workspace\jenkins-git
cd C:\Windows\System32\config\systemprofile\AppData\Local\Jenkins.jenkins\workspace\jenkins-git
%T:~0,-4%.exe
del nihao.txt
pause
del %T:~0,-4%.exe 
pause'"
                    }
                }
            }
        }
    }
}
