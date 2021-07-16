#to login to ecr
aws ecr get-login-password --region us-east-2 | sudo docker login --username AWS --password-stdin 478208517748.dkr.ecr.us-east-2.amazonaws.com
sudo docker build -t 478208517748.dkr.ecr.us-east-2.amazonaws.com/jquery-eks:$BUILD_NUMBER .
sudo docker push 478208517748.dkr.ecr.us-east-2.amazonaws.com/jquery-eks:$BUILD_NUMBER 



ingress-controller----->load balancer

deployed the
-->namespace
-->deployment
-->service
-->ingress
