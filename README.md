# Active-Directory-Home-Lab

<h1>Project Overview</h1>
<p>
    I set up an Active Directory lab environment on my personal computer using Oracle VirtualBox. This project involved creating a virtualized network that simulates a corporate environment, allowing for practical experience with Windows networking and Active Directory services utilizing two Virtual Machines.
</p>

<h1>Skills and Technologies Used</h1>
<ul>
    <li><strong>Virtualization:</strong> Proficient use of Oracle VirtualBox for creating and managing virtual machines.</li>
    <li><strong>Windows Server Administration:</strong> Installation and configuration of Windows Server 2019.</li>
    <li><strong>Active Directory Management:</strong> Setup and administration of Active Directory Domain Services.</li>
    <li><strong>Networking Fundamentals:</strong>
        <ul>
            <li>IP addressing and subnetting.</li>
            <li>Configuration of NAT, DHCP, and DNS services.</li>
            <li>Understanding of routing and remote access.</li>
        </ul>
    </li>
    <li><strong>Automation with PowerShell:</strong> Writing scripts to automate administrative tasks in Windows environments.</li>
    <li><strong>Client-Server Architecture:</strong> Experience with domain joining and client-server interactions in a Windows network.</li>
</ul>


<h1>Key Components and Steps</h1>

<h2>1. Virtualization with Oracle VirtualBox</h2>
<ul>
    <li>Installed Oracle VirtualBox and the Extension Pack.</li>
    <li>Configured virtual machines (VMs) for both a domain controller and a client machine.</li>
</ul>

<h2>2. Operating Systems Installation</h2>
<ul>
    <li>Downloaded and installed Windows Server 2019 on the domain controller VM.</li>
    <li>Downloaded and installed Windows 10 on the client VM.</li>
</ul>

<h2>3. Network Configuration</h2>
<ul>
    <li>Set up two network adapters on the domain controller VM:
        <ul>
            <li>One connected to the external internet (NAT).</li>
            <li>One connected to an internal VirtualBox network for client connectivity.</li>
        </ul>
    </li>
    <li>Assigned static IP addresses and configured network settings to enable communication between VMs and internet access.</li>
</ul>

<h2>4. Active Directory Domain Services (AD DS)</h2>
<ul>
    <li>Installed AD DS on the Windows Server 2019 VM.</li>
    <li>Created and configured my own example Active Directory domain (<code>mydomain.com</code>).</li>
</ul>

<h2>5. Routing and Remote Access Service (RRAS)</h2>
<ul>
    <li>Configured NAT and routing on the domain controller to allow client machines to access the internet through the internal network.</li>
</ul>

<h2>6. DHCP and DNS Setup</h2>
<ul>
    <li> I then Installed and configured DHCP on the domain controller to automatically assign IP addresses to client machines.</li>
    <li>Configured DNS services to resolve domain names within the network.</li>
</ul>

<h2>7. PowerShell Automation</h2>
<ul>
    <li>I executed a PowerShell script to create 1,000 user accounts in the Active Directory automatically.</li>
    <li> The Script included parameters for usernames, passwords, and organizational units.</li>
</ul>

<h2>8. Client Machine Configuration</h2>
<ul>
    <li>Set up a Windows 10 VM as a domain-joined client machine.</li>
    <li>Configured network settings to obtain an IP address from the DHCP server.</li>
    <li>Joined the client machine to the (<code>mydomain.com</code>) domain.</li>
    <li>Lastly, I tested and verified the user authentication by logging in with a few domain user accounts.</li>
</ul>

<!--
1
--!>
