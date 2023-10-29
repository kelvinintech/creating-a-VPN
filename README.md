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
  For the image<b>(Base operating system or application for the VM)</b> select <b>Windows 10</b>
  <BR /><img width="519" alt="SECURITY TYPE" src="https://github.com/codeByKelvinn/creating-a-VPN/assets/110644520/58b5272c-eb64-4691-ab16-70da26837a5c">

</P>
