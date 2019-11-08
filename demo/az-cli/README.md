# How to create a Linux VM on Azure using CLI

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

*Be aware that this script uses the resource group name, location and virtual machine name as paramaters*

```bash
bash createvm.sh rg-cli eastus vm-01
```



