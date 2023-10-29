# creating-a-VPN


<p>
<b>What is VPN and why do I need it?</b>

<br />A VPN, which stands for virtual private network, establishes a digital connection between your computer and a remote server owned by a VPN provider, creating a point-to-point tunnel that encrypts your personal data, masks your IP address, and lets you sidestep website blocks and firewalls on the internet.
</p>



<p>
The initial action in this process is to visit www.whatismyipaddress.com. Once there, you'll be required to obtain your IP address. Ensure that you save a copy of your IP address in a separate document for future reference. Copy the IPv4 address specifically

![whatismyipaddress](https://github.com/codeByKelvinn/creating-a-VPN/assets/110644520/e5d68d91-911f-40a3-a4fd-249f5c704c5c)

</p>


<p>


![whatismyipaddress 2](https://github.com/codeByKelvinn/creating-a-VPN/assets/110644520/15db5a19-f1d3-4a6f-888c-870048ec6bfb)


</p>

<p>

The subsequent action involves visiting portal.azure.com and initiating the creation of a virtual machine. Navigate to Azure Services on the Azure homepage and select Virtual Machines. 
<br />
![creating a vm 1](https://github.com/codeByKelvinn/creating-a-VPN/assets/110644520/1f909643-5e7b-4a2c-abef-b3e11854755e)

Click on 'Create' denoted by the + symbol, then choose the Azure Virtual Machine option. Look for the small text stating 'Create a virtual machine hosted by Azure' and proceed by selecting that.
<br />
<img width="194" alt="creating a vm" src="https://github.com/codeByKelvinn/creating-a-VPN/assets/110644520/4b738e21-fa95-4929-b566-4e94c7036515">

</p>

<p>

  Permit Azure to generate the resource group on your behalf. Typically, it will opt for the name you've chosen for your virtual machine
  <br />

<img width="572" alt="creating a vm 2 " src="https://github.com/codeByKelvinn/creating-a-VPN/assets/110644520/ba2ed3f0-e0de-4dd8-a782-a1d91a8ad8df">

<br />

</p>


<p>

 <bold>NOTE! MAKE THE REGION SOMEWHERE DIFFERENT FROM WHERE YOU LIVE!!</bold>
  I'm in Atlanta, GA so I chose WEST US
<br />
<img width="462" alt="region" src="https://github.com/codeByKelvinn/creating-a-VPN/assets/110644520/373f532f-1922-46bc-9ee0-a47980bf991f">
<br />

</p>

<p>

 <bold>For the Availability Options select <b>No Infrastructure Redundancy Required</b> from the dropdown menu
 <br />
<em>
<img width="408" alt="availability" src="https://github.com/codeByKelvinn/creating-a-VPN/assets/110644520/de4c501c-a061-4e0f-8dc8-2cef84abee81">


<br />
Azure offers a range of options for managing availability and resiliency for your applications. Architect your solution to use replicated VMs in Availability Zones or Availability Sets to protect your apps and data from datacenter outages and maintenance events.</em>

<br />


<br />

</p>


<P>
  Security type should be set to <b>standard</b>
  <br />

  
  <i>Security type refers to the different security features available for a virtual machine.</i>
  <br />

  
  For the image<i>(Base operating system or application for the VM)</i> select <b>Windows 10</b>

  
  <BR /><img width="519" alt="SECURITY TYPE" src="https://github.com/codeByKelvinn/creating-a-VPN/assets/110644520/58b5272c-eb64-4691-ab16-70da26837a5c">

</P>


<p>
  select Review + create in bottom corner

  
  <br />

  
  <img width="463" alt="review and create" src="https://github.com/codeByKelvinn/creating-a-VPN/assets/110644520/a6cb46db-e34a-4a6f-8887-b23cb69af356">

</p>



<p>

  After the deployment finishes, return to the main Azure screen by clicking on "Microsoft Azure" located at the top left corner. From there, choose "Virtual Machine" to access the VM you've just created. You can also reach the Virtual Machine via the search bar at the top.
  
  <br />
  <img width="479" alt="deployment complete" src="https://github.com/codeByKelvinn/creating-a-VPN/assets/110644520/3961ad3a-e0a7-415d-8bcd-a8da827924b9">


 Access the VM you just made and copy your public IP address
 <br />
 
<img width="948" alt="vm practice public id" src="https://github.com/codeByKelvinn/creating-a-VPN/assets/110644520/8ec87936-b65a-4d62-bf5b-d6197de3ad15">

</p>


<p> 
  
  Go to your search bar to access Remote Control Desktop
  
  <br />
  
  <img width="260" alt="remote desktop" src="https://github.com/codeByKelvinn/creating-a-VPN/assets/110644520/154c7650-9743-41fa-88a6-a5cc7ec8ff1c">

Paste your IP address in the proper field 
<br /><img width="302" alt="VM IP HERE" src="https://github.com/codeByKelvinn/creating-a-VPN/assets/110644520/a10dd6d4-575b-4194-b332-1b79799a3623">


</p>
You will be prompted to enter your credentials. Select <b>more choices</b> at the bottom
<img width="337" alt="more choices" src="https://github.com/codeByKelvinn/creating-a-VPN/assets/110644520/c5fe4693-2764-4cdb-a0e4-e7c29c49db60">

<p>
  Once you see this window, accept the certificate. Then you will be connected.
  
<br /><img width="332" alt="accept certificate" src="https://github.com/codeByKelvinn/creating-a-VPN/assets/110644520/d72c0ee5-bde2-4b41-8f65-800a93af12bc">

</p>


<p>
  Disable all settings once this menu appears. Then, click <b>accept.</b>
  <br /><img width="514" alt="disable" src="https://github.com/codeByKelvinn/creating-a-VPN/assets/110644520/63791dd0-94a6-43d6-8d7f-5b2e98e2fc43">

</p>

<p>
  Next you are going to return to https://whatismyipaddress.com/ but this time, you are going to it in your virtual machine. If you are a bit confused as to which is your VM and your PC, Your VM will have the IP address at the top of the browser
  <br />
  <img width="960" alt="whole screen" src="https://github.com/codeByKelvinn/creating-a-VPN/assets/110644520/af3dcac6-e0c0-494c-9d93-ecb80bd1bb29">

</p>


  <p>
Duplicate your VM's IP address and insert it into the notepad document you previously utilized.
  <br />
    <img width="350" alt="notepad vm" src="https://github.com/codeByKelvinn/creating-a-VPN/assets/110644520/c4effee0-477e-4749-b74c-7df36942400d">

</p>



  <p>
    Within your PC, you are going to sign up for Proton VPN.
    <br /><img width="90" alt="PROTON VPN" src="https://github.com/codeByKelvinn/creating-a-VPN/assets/110644520/6fd9e26c-9028-4678-b507-3fea954f43e5">
    Once we sign up, were going <b>back</b> to https://whatismyipaddress.com/
  <br />

  Once you have accessed https://protonvpn.com/ create an account
<br />
<img width="839" alt="proton vpn 2" src="https://github.com/codeByKelvinn/creating-a-VPN/assets/110644520/1620874e-7679-4a64-8436-8f6fbbfc19ed">

</p>



  

