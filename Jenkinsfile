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
                sh """
                    sudo apt-get install nginx -y
                    
                    sudo systemctl start nginx
                    
                    cd /var/www

                    rm -rf html 

                    sudo mkdir html

                    cd html

                    sudo git clone https://github.com/seunhub007/simple_devops.git .

                    

                    """

            }
        }
    }
}