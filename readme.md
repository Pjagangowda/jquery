aws ecr get-login-password --region us-east-2 | sudo docker login --username AWS --password-stdin 002784619873.dkr.ecr.us-east-2.amazonaws.com

sudo docker build -t 002784619873.dkr.ecr.us-east-2.amazonaws.com/jquery-eks:$BUILD_NUMBER .

sudo docker push 002784619873.dkr.ecr.us-east-2.amazonaws.com/jquery-eks:$BUILD_NUMBER