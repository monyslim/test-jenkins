pipeline {
    agent any

    stages {
        stage("getting the source code"){
            steps{
                echo "Getting the source code"
            }
        }

        stage("building the image"){
            steps{
                echo "Build the image"
            }
        }

        stage("running the image container"){
            steps{
                echo "container is running ...__-"
            }
        }

        stage("host website"){
            steps{
                sh  '''
                        sudo apt-get install nginx -y
                        
                        sudo systemctl enable nginx
                        
                        sudo systemctl enable nginx
                        
                        cd /var/www

                        sudo chown -R jenkins:jenkins wwww/

                        rm -rf html 

                        mkdir html

                        sudo chown -R jenkins:jenkins html/
                        
                        cd html

                        git clone https://github.com/monyslim/test-jenkins.git .

                    

                    '''

            }
        }
    }
}