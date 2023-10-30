# creating-a-VPN

<p>

  Learning to use a Virtual Private Network (VPN) is often necessary for an IT professional due to various reasons.
  <br />
  <b>Remote Access</b>: Helpdesk support often requires accessing internal company systems and tools. A VPN allows secure access to these resources remotely, especially if the helpdesk team members are not physically present in the office.

<b>Security and Privacy</b>: Using a VPN ensures that data transmitted between the helpdesk support agent's device and the company's network is encrypted and secure. This is crucial when handling sensitive information or accessing company systems to avoid potential security breaches.

<b>Client/Company Confidentiality</b>: Helpdesk support may involve handling proprietary or confidential information. Using a VPN helps maintain the confidentiality of data and communications, ensuring that customer and company information remains protected.

<b>Access Control and Compliance</b>: Companies often have access restrictions or compliance requirements. A VPN enables helpdesk employees to comply with these access control measures, allowing them to securely connect and work within the company's network without violating security protocols.

<b>Experience and Troubleshooting</b>: Familiarity with VPNs might also be essential when providing support to customers who use VPNs themselves. Understanding how VPNs work can help troubleshoot connectivity issues or guide users through setting up their VPN connections.
</p>

<p>

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Proton VPN https://protonvpn.com/
  
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
    <br />
    Once we sign up, were going <b>back</b> to https://whatismyipaddress.com/
  <br />

  Once you have accessed https://protonvpn.com/ create an account  
  
<br />

<img width="839" alt="proton vpn 2" src="https://github.com/codeByKelvinn/creating-a-VPN/assets/110644520/1620874e-7679-4a64-8436-8f6fbbfc19ed">

You will see pricing options. Click "Get Proton Free"
<img width="880" alt="proton vpn 3" src="https://github.com/codeByKelvinn/creating-a-VPN/assets/110644520/cb508c6f-fd82-403c-b3df-4ee18dd60f3a">
</p>

<p>Once you have signed into Proton on your machine, take the URL, which would be 
  <br /> 
  https://account.protonvpn.com/downloads 
<br /> Copy it, and paste it into your VM's browser, then sign in using the same credentials for Proton
 
  <br /> <img width="958" alt="vpn whole screen" src="https://github.com/codeByKelvinn/creating-a-VPN/assets/110644520/6d14c8d7-fb08-4f89-9b73-bd0e564038ca">


Once in your Virtual Machine and signed into Proton, download the Windows VPN 

<br /> <img width="539" alt="vpn download windows" src="https://github.com/codeByKelvinn/creating-a-VPN/assets/110644520/cf681992-f0a8-4234-a191-3b84c17a0f6b">


Click Download Proton VPN 

<br /><b>Remeber, you are in your VM, not your PC</b>
<br /><img width="182" alt="download windows vpn" src="https://github.com/codeByKelvinn/creating-a-VPN/assets/110644520/03d76e18-6005-4280-9798-5a2c167c99c0">

Accept all the default settings and proceed with download
<br /> 
<img width="488" alt="vpn defaults" src="https://github.com/codeByKelvinn/creating-a-VPN/assets/110644520/a0a9799c-f82f-48a8-93a7-3779495647d2">

log in with the same <b>Proton</b> credentials
<br /> <img width="600" alt="proton credentials" src="https://github.com/codeByKelvinn/creating-a-VPN/assets/110644520/47128871-5462-4965-870f-161d30a74f66">

Once logged in select Japan as the server. Do not select <b>Quick Connect</b> for this exercise
<br /><img width="467" alt="vpn japan connect" src="https://github.com/codeByKelvinn/creating-a-VPN/assets/110644520/b88608fb-d4eb-4d31-9542-6831c69a9024">

<br /> <i>I've stopped using the quick connect to fastest, because I found it connected to servers that were abnormally slow</i>

<h3>Once you connect to the Japan server(or quick connect/whatever server you selected), it is essentially creating a tunnel to a server in Japan</h3> 

<br />The image below is a illustration of the what is happening

<br /><img width="622" alt="vpn illustration" src="https://github.com/codeByKelvinn/creating-a-VPN/assets/110644520/f8e9f2fb-098b-4cbb-9ae5-664739e211da">

The server will begin loading. 
<br /> You can tell if the connection is dropped because the screen will freeze is some cases

<br /><img width="400" alt="vpn server loading" src="https://github.com/codeByKelvinn/creating-a-VPN/assets/110644520/19171b90-c9a6-4a0f-85c7-57f7841fd36a">

Once this screen has displayed again,  you are offically connected to the server
<br /><img width="470" alt="vpn japan connect 2" src="https://github.com/codeByKelvinn/creating-a-VPN/assets/110644520/e7db7c31-27e4-48e4-8dbc-fb2cbdabd5b0">

<br /><i>congratulations</i>

On our Virtual Machine we are going <b>back</b> to https://whatismyipaddress.com/

<img width="623" alt="VPN SETTINGS CHANGED" src="https://github.com/codeByKelvinn/creating-a-VPN/assets/110644520/950003ed-e2e6-4ace-9a56-1fd9696b15a3">


The IP address and location should be of your newly established VPN created in Proton
<i>if you selected Japan in Proton, to go https://www.google.com and it should be in Japanese.</i>
</p>


  <h4>There you go! You've successfully created a VPN! Hope this was helpful. If you have any questions or concerns, feel free to message me. Take care!</h4>

  

