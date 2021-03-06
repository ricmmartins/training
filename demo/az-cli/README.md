# How to create a Linux VM on Azure using CLI

This demo will deploy an Ubuntu Server with PHP, Nginx and an [application](https://github.com/ricmmartins/simple-php-app) deployed.

From the Azure portal, let's open the Cloud Shell

<img src=../az-cli/pictures/1.png>


<img src=../az-cli/pictures/2.png>

When the Cloud Shell be ready, download the following script: [https://github.com/ricmmartins/azure-arm-template/blob/master/createvm.sh](https://github.com/ricmmartins/azure-arm-template/blob/master/createvm.sh)

To do this, run the following command:

```bash
wget https://raw.githubusercontent.com/ricmmartins/azure-arm-template/master/createvm.sh
```

<img src=../az-cli/pictures/3.png>

Now lets run the script:

*Be aware that this script uses the resource group name, location and virtual machine name as paramaters. So you need to run as below:*

```
createvm.sh <resource group name> <location> <vmname>
```

In this case:

```bash
bash createvm.sh rg-cli eastus vm-01
```

So after a few seconds we can see as below:

<img src=../az-cli/pictures/4.png>

Then we can go to resource group, select the VM and get their public ip address to access:

<img src=../az-cli/pictures/5.png>

<img src=../az-cli/pictures/6.png>

Lets check:

<img src=../az-cli/pictures/7.png>






