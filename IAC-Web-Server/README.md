To set up infrastructure as code (IAC) for running a website using Vagrant, follow these steps:

#### Download and Install Vagrant:
Go to the Vagrant website, download the appropriate version for your operating system, and follow the installation instructions.

#### Create a Folder :
Create a new folder on your computer where you want to store your Vagrant configuration files. You can name it something like "iac_website_vagrant".

#### Copy Vagrantfile :
 Locate the vagrantfile in the IAC Web folder, it contains the configuration for your Vagrant environment. Copy the Vagrantfile and paste it into the folder you created earlier ("iac_website_vagrant")

#### Run vagrant up :
Open a terminal or command prompt, navigate to the folder where you placed your Vagrantfile ("iac_website_vagrant"), and run the command: "vagrant up"

This command will create and provision the virtual machine . It may take some time depending on your internet connection speed and the complexity of your setup.

#### SSH into the Virtual Machine:
Open a terminal or command prompt, navigate to the folder where your Vagrantfile is located, 
and run: "vagrant ssh"
This command will connect you to the virtual machine via SSH.

#### Locate ip address of website:
Once you're logged into the virtual machine, run the following command to display the network interfaces and their associated IP addresses: "ip addr show"
This command will show you the IP addresses assigned to the network interfaces on the virtual machine.

#### Identify the IP Address :
Look for the IP address associated with the network interface that you want to use to access your website. This could be the IP address assigned to the primary network interface (often named eth0 or enp0s3).

#### Access the Website :
After identifying the IP address, open a web browser on your host machine and enter the IP address in the address bar, followed by the appropriate port if necessary. For example, if the IP address is 192.168.80.10 and your website runs on port 80, you would enter http://192.168.80.10 in the browser address bar.

By following these steps, you should be able to locate the IP address of your virtual machine provisioned by Vagrant and access your website in a browser.