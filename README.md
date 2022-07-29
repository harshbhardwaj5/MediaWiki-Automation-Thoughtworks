# MediaWiki-Automation-Thoughtworks
Automation of mediawiki task for thoughworks
Getting Started
Follow these simple instructions to get your minkikube up and running along with Mediawiki deployed into it.

Prerequisites
Install Terraform and git on the machine.
Install ruby and ruby json.
Export the ACCESS KEY and SECRET KEY of AWS as an environment variable or pass it during the run time
yum install git ruby ruby-json -y
wget https://releases.hashicorp.com/terraform/0.12.6/terraform_0.12.6_linux_amd64.zip
sudo unzip ./terraform_0.11.13_linux_amd64.zip -d /bin/

Running The Automation
Clone the current repo to your local machine using
git clone https://github.com/Anurag-30/MediaWiki.git

Move into Terraform directory
cd MediaWiki/Terraform/

Run the Terraform script
terraform apply

Need to specify the region at the run time eg:us-east-1.

You will get the ssh key into wikimedia file with which you can login into the ec2 machine that has been launched. You can access the application at http://{publicip}:30163/wiki

