Objectives:
1.	To know about basic networking commands and famalier with it.


Theory and Lab Activities:
•	Open Windows cmd.
•	Type the following commands.

# 1. PING
 Used for: Finding and Troubleshooting network connection status/ issues.
Cmd to enter: ping
When determining if two network hosts can interact with one another, Ping is employed.
The device will respond to the ping with four data packets if nothing stands in the way of the ping reaching its target, such as a firewall or a network issue.
The ping verifies that there is a functional network path between you and the destination host if you get these packets back.
 

# 2. IPCONFIG
Used for: Finding your IP address
Cmd to enter: ipconfig
The fundamental IP address configuration data for the Windows device you're working on is displayed by IPConfig Cmd.
IPConfig has a few switches  to provide additional information  actions:

•	IPConfig /all – Displays additional information for all network adapters
•	IPConfig /release – Releases the IP address you are currently using
•	IPConfig /renew – Renews an IP address on your device
•	IPConfig /flushdns – Flushes the DNS cache
•	IPConfig /? – Displays help for IPConfig and its switches

 


# 3. ARP
Used for: Resolving problems with network connections
Cmd to enter: arp
Address Resolution Protocol, or ARP, is used by the Cmd to translate an IP address to a MAC address.
It is simple to believe that all network communication uses IP addresses, however this is not the reality. The network adapter's MAC address, not its IP address, ultimately determines whether packets are delivered to a device.

# 4. GETMAC
Used for: Finding your MAC address quickly
Cmd to enter: getmac
In order to be compliant with the IEEE 802 standards, each device must have a unique MAC (Media Access Control) address. 
The manufacturer of your device will assign it a MAC address and store it within the hardware.
The getmac Cmd provides an easy way to find the MAC address of your device. If you see more than one MAC address for your device, it will have multiple network adapters. As an example, a laptop with both Ethernet and Wi-Fi will have two separate MAC addresses. 



# 5. HOSTNAME
Used for: Finding your MAC hostname quickly
Cmd to enter: hostname
You can quickly determine the hostname that has been assigned to your Windows device using the hostname Cmd.
Although there are methods for finding this in Windows, using the Cmd line is much quicker.



# 6. NSLOOKUP
Used for: Resolving problems with network connections
Cmd to enter: nslookup
For identifying DNS name resolution issues, utilize NSLookup.
You may find the name and IP address of your device's DNS server by typing nslookup at the Cmd prompt.
This will most likely be your router for you at home, but in business settings, it will usually be a dedicated DNS server. 

 

# 7. NBTSTAT
Used for: Resolving problems with  NetBIOS,
Cmd to enter: nbstat
The device will also have a domain or workgroup allocated to it, to which it belongs. Your device is probably in its own workgroup for you at home.
The NetBIOS name, which is where the nbtstat Cmd comes into play, is the technical term for the computer name.
Windows uses a variety of techniques, such as broadcast and LMHost search, to connect NetBIOS names to IP addresses.
The nbtstat Cmd is used to assist you identify and fix these issues because this mapping occasionally fails.
The nbtstat -r Cmd displays how many NetBIOS names a device has recently been able to access, whereas nbtstat -n displays the NetBIOS names that are now being used by a device.
 
# 8. NET
Used for: a list of available Net switches
Cmd to enter: net
The net Cmd is undoubtedly an useful tool that enables you to handle a variety of network settings and characteristics, including network shares, users, and print jobs, to name a few.
Even while running only net won't accomplish much, it will list every switch that is available.
Accounts can be used to provide password and logon requirements, files can display a list of open files, and sessions can list or even end network sessions.
Run net help to find out what each switch does if you're ever unsure. I'm confident you'll get the answer.
# 9. NETSTAT
Used for: network statistics display
Cmd to enter: netstat
Viewing network statistics is an excellent tool to troubleshoot any issues your network is having and may very well help you identify the source of the issue.
This is exactly what the netstat Cmd does—it gives you a helpful network summary for your device.
A list of connections that are active and being added to every few seconds can be found by running netstat.
The protocol that is being used, the local address, the foreign address, and the connections state will all be described.
Use the netstat -e switch to view some interface statistics, such as bytes sent and received, errors sent and received, and unidentified protocols.

# 10. NETSH
Used for: showing and setting up network adapters
Cmd to enter: netsh
Another extremely potent command is netsh, which gives you much more detailed access to practically all of the network adapters in your device than some other commands.
The Cmd prompt will go into network shell mode when you run the netsh Cmd on its own. There are various "contexts" inside this mode, including ones for DHCP-related tasks, diagnostics, and routing.
However, it is still possible to execute specific commands directly from netsh.
Run netsh / to view all of the available netsh contexts.
Run netsh contextname /? to view all of the commands accessible within that context.
Some commands have the option of subcommands.
Run netsh contextname show / to see these.

# 11. TASKKILL
Used for: Ending processes
Cmd to enter: taskkill
You probably already know that you can terminate a process using the Task Manager, but did you also know that you can do so from the Cmd line?
You absolutely can, and you have the choice to terminate a task or process using the file name or the process ID.
Use the tasklist Cmd to first see the process name (shown as the image name) and how much memory that process is using if you are unsure of which processes are running and hence what has to be stopped.
Once you are aware of the process's name, you can terminate it with taskkill /IM processname.exe.



# 12. TRACERT
Used for: resolving problems with network connections
Cmd to enter: tracert
You may examine information on each "hop" along the route and follow the path that a packet travels to get to its destination by using the tracert Cmd.
A hop is the quantity of routers a packet travels through on its way. When a packet travels through additional networking hardware, such as repeaters, switches, and access points, a hop may or may not be counted. This depends on how these devices are set up and what function they serve on the network.
Following the execution of the tracert command, you will be shown a line-by-line summary of each hop, along with the IP address and the latency between your device and that specific hop.


# 13. PATHPING
Used for: resolving problems with network connections
Cmd to enter: pathping
The parallels between the ping and tracert commands have already been discussed.
As you might have guessed from the command's name, pathping combines the best features of ping and tracert into a single utility.
When you type pathping into the Cmd prompt after a hostname, it starts what appears to be a standard tracert command.
 

# 14. SYSTEMINFO
Used for: Displaying system information
Cmd to enter: systeminfo
You may access all of this information through the Windows GUI if you need to know anything specific about the device you are using, including information on the processor it is running, the version of Windows you are using, or how the boot device is set up.

# 15. NET VIEW
Used for: Viewing devices connected to a network
Cmd to enter: net view
You might occasionally want to know which devices are linked to your network. The net view Cmd can be useful in this situation.
You may see a list of the devices that are connected to the same network as you by simply running the net view Cmd.
It should be noted that this Cmd might not display all of the devices connected to your network.


# Observation and Conclusion:
-	Learned to applications of  various network commands
