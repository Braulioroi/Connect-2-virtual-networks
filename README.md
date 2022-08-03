## Connect 2 virtual networks
We enter the Azure portal and go to the virtual networks section, we create a new virtual network, we fill in the basic data (subscription, resource group, network name and region)

![](/imagenes/1.PNG)

We go to the ip addresses section and add a subnet with address 10.0.0.0/24 and with that we create our first virtual network virtual network

![](/imagenes/2.PNG)

We repeat the previous steps and create our second virtual network with subnet address number 10.1.0.0/24

Then we create 2 virtual machines adding the basic data and the networks to which they will be connected, one to virtual network 1 and the other to virtual network 2 (note that the networks and virtual machines are in the same region)

![](/imagenes/4.PNG)
![](/imagenes/5.PNG)
![](/imagenes/6.PNG)
![](/imagenes/7.PNG)

We go to any virtual network and we click on the pairing section, there we fill in all the data and we click on add pairing

![](/imagenes/3.PNG)
![](/imagenes/10.PNG)
![](/imagenes/11.PNG)

Once all the resources have been created, we go to the first virtual machine in the connect section and copy the command to connect to the virtual machine

![](/imagenes/8.PNG)

We enter the Azure PowerShell we write ssh and the copied command will ask you if you want to continue connecting the virtual machine we write yes, the user will appear and it will ask us for the password we write it and we will enter the virtual machine

![](/imagenes/9.PNG)
![](/imagenes/12.PNG)

Once inside we perform a ping to the other virtual machine and thus verify that the two networks are connected