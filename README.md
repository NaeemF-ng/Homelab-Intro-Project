### Homelab-Intro-Project
![Homelab overview](./images/All-VM's.png)

This is just visual of all of the VM's that I have in my homelab as of right now, i'll add more to it throughout my cyberjourney. 

![Kali settings](./images/Kali-Settings.png)

I have my kali machine ON the NAT Network setting which allows for it coomunicate with other VM's in my homelab and they aren't exposed to the real internet. I had made a new NAT Network called "Labnet" so it doesn't interfere with my ISP as I was having problems with this recently on my newest addition opnsense. I would try to visit an IP and it would direct me to an ISP page, which wasn't supposed to happen but when I created the labnet NAT Network and added all of the other VM's I was using to it as well, the problem was solved. This is where I spend most of my time, on the kali machine.

![Metasploitable3 settings](./images/Ms3Settings.png)

I have the metasploitable3 machine on the Labnet NAT Network also to keep it away from the internet as it intentionally has vulnerable services so that it can be practiced on. This is always my target VM when i'm looking to practice pentesting techniques and things of that nature.

![Ubuntu Settings](./images/Ubuntu-Settings.png)

The ubuntu machine is also on the Labnet NAT Network kept away from the internet. I use it to just run scans against it for the most part.However when I was trying to create my first personal project I was using to mess around with firewalls via the ufw command, I'll try to incorporate this VM more into future projects.

![Kali Scans](./images/Kali-Scans.png)

I used my kali machine to scan both the ubuntu and metasploitable machines via the following commands: 
- ping -c 3 <metasploitable ip>
- ping -c 3 <ubuntu ip>

**note**: This command is used to see if a machine is up and running and can be reached. The -c argument is used to specify how many packets we want to send to the machine that is being pinged. Lastly, the results say 3 packets were sent and 3 were received meaning that the host is up, had the host not been up, it would've said no packets were received.









This personal project will be explaining what I use to conduct safe and ethical hands on learning in a controlled environment such as my homelab. I'll touch on what virtual machines I use, architecture, configs, settings, etc.
