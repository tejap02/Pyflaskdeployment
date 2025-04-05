# Pyflaskdeployment
Frist Clone the repo

cd pyflaskdockerapp
ls
cat dev.bat
# check for opreating system
cat /etc/os-release(check for opreating system)
# for check the version
cat > version.txt 
4.0.1
# docker login
# build the image
$docker build -t custom-img-pyapp:$(cat version.txt) .
# check the images
$docker images
# Create the container
$docker run --rm -p 8000:8000 custom-img-pyapp:$(cat version.txt) .
# check the running conatiner & all container
$docker ps
$docker ps -a
# install aws cli 
# awx --version
# aws configure
# add secrect access key/id
# exit pyflaskapp folder
cd..
cd pyflaskapp
# before push the images tag the image
$docker tag 
# push the image Amazon Elastic Container Registry (ECR).
aws ecr get-login-password --region <your-region> | docker login --username AWS --password-stdin <aws-account-id>.dkr.ecr.<your-region>.amazonaws.com







