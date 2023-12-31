<h1>VM Creation and Connection Lab(Azure)</h1>

<h2>Description</h2>
Welcome to my virtual lab, where we're discovering Microsoft Azure together. In this lab, we're learning how to create virtual machines using Azure and connect to them using Remote Desktop. It's an exciting journey into the world of IT, join me as we build our IT skills, one step at a time. It's a beginner-friendly space, so don't hesitate to jump in and start learning with me!
<br />


<h2>Languages and Utilities Used</h2>

- <b>Microsoft Azure</b> 
- <b>Remote Desktop Connection</b>

<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)
- <b>Ubuntu<b> (x64 Gen2)
<h2>Program Walk-Through:</h2>
<p align="center">
First Step On Creating Your VM👨‍💻
 
<p>
Once you login into your azure account, you will go to the icon "virtual machine" and press create. 
</p>
<br />

 ![Create Icon for VM](https://github.com/nw4466tu/VM-Connection-Lab/blob/main/Create%20VM%20icon.PNG?raw=true)
<br />
<p>
Pick the subscription you are using for the lab, and then either choose an existing reasource group or create a new one. Next you will name your VM, in my case I named it VM1. You can use any region, but just for me it worked best when I used US West 3. Since we are making two different virtual machines, my first one will be Windows 10 with VM architecture x64. When choosing the size it just depends on how fast you want your VM to be, certain ones will require more cpus, but in my case 2cpus with 16 GiB memory worked perfectly fine. After this it will have you make a username and password for your VM (DO NOT FORGET THIS!!) so that you can login and in later projects, so that you can read the traffic using these items. Allow select ports and makes sure the inbound port is RDP (3389) and check the box. After this we will hit the next/disk then go next to networking where it'll create a subnet, IP address, NSG(firewalls), and NIC for our Windows VM, click create where it'll validate it and the click create icon one more time.
</p>
<br />

![Creating our VM](https://github.com/nw4466tu/VM-Connection-Lab/blob/main/Creating%20a%20VM%20in%20Azure.PNG?raw=true)![Creating or VM2](https://github.com/nw4466tu/VM-Connection-Lab/blob/main/Creating%20a%20VM%20in%20Azure%20(2).PNG?raw=true)![Networking Interface](https://github.com/nw4466tu/VM-Connection-Lab/blob/main/Creating%20a%20Subnet%20and%20IP%20address%20for%20Windows%20VM.PNG?raw=true)



<br />
<p>
After your VM is created, continue the same process where we're using the same resource group, region, and naming this one VM2. Since we're going to connect to Ubuntu in this lab, we are going use Ubuntu x64 Gen2 for the server. And instead of using SSH public key for authentication type, we're going use password (same as VM1) since we're connecting over SSH. Keep SSH(22) as your inbound port as well as the same size of cpus. Click next for discs, then click to networking where it should automatically select the same virtual network, subnet, and IP address. Click create, it should pass the validation and then click create one more time. 
</p>
<br />

![Creating our VM](https://github.com/nw4466tu/VM-Connection-Lab/blob/main/Ubuntu%20VM%20Picture.PNG?raw=true)



<br />
<p>
Once created, search virtual machines and click on VM1 where you will look for your public IP address and copy it. Go to your search bar and type in Remote Desk Top and then paste the IP address in there, click connect, and there should be a Windows security screen asking for you username and password. You might have to search for it if it doesn't come right up on the screen. If that's the case, go to more choices and click use a different account and type in the username and password you created for these VM's. After you do this, you'll probably get a warning message saying it's not trustworthy, but just click yes and you should be connected to your very own virtual machine.
<br/>
<br />
<br />
<br/>
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
