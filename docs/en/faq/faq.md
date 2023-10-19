## Is Amnezia a VPN service?
  No Amnezia is not a VPN-service, it's a VPN-client with which you can set up and use your own VPN.

## Is Amnezia a free service?
  Yes, Amnezia is completely free software. You don't need to connect to our servers, and you don't have to pay anything to us. However, in order to create your own VPN, you will need to purchase a VPS from any provider or use an existing one.

## Which devices and operating systems does Amnezia support?
  Currently, there are versions available for Windows, macOS, Android, iOS, and Linux.

## Does Amnezia collect user data?
  Amnezia does not collect or transmit any statistics, logs, analytics, or other user information. The only data the client requests is connection data. This data is also not collected or transmitted, which can be verified due to the open-source of both the server and client software.

## How does Amnezia work?
  You provide the IP address, login, and password of your server. The application connects to the server via SSH, installs Docker, and launches Amnezia server containers. Separate containers are created for each connection protocol, and keys and root certificates are generated. Once the server is configured, you can connect to it via VPN.

## Why Amnezia is more resistant to blocking than other VPNs?
  The larger and more popular a commercial VPN service becomes, the more likely it is to attract attention from surveillance agencies and authorities, increasing the chances of its servers and protocols being blocked.

## What are the advantages of Amnezia and other Self-hosted VPN services over regular VPN?
**Full Control** - you have full control over your own VPN server, including configuration, security, logging, and data access. You have the ability to choose the configuration, encryption protocols and security settings according to your requirements.

**High performance** - self-hosted VPN can offer better speed and performance because you control the server resources and can customize it to your needs. This is especially useful if you have a large number of users or require high bandwidth.

**Bypass restrictions** - many sites know the IP addresses of popular VPN servers and blacklist them. When you buy a separate VPS, your IP address is known only to you and those with whom you have shared your connection data.

**Mobility** - you can use your configured VPN not only with the Amnezia client but also with other self-hosted applications that support selected VPN protocols.

## I downloaded the app, what's next?
  Once you have downloaded the app, you need to enter your VPS details. You can use your existing VPS or buy a new one. As an example, here are the instructions for buying a VPS on several popular hostings.
## I want to buy a VPS, what options should I choose?
 Amnezia works with any KVM virtualization servers running Ubuntu (officially supported version is 20.04) and Debian 10.

## Why do I need a server with KVM?
 Amnezia uses Docker to stand-alone your VPN server deployment. Not every type of virtualization can be used with Docker, but KVM definitely allows it. Other types of virtualization may not work with Docker, either due to the limitations of the specific virtualization type or due to configuration from the VPS vendor.

## Which VPN protocol to choose?
**IMPORTANT!** If your country has a very high level of control and blocked access to many sites, do not work any commercial and free VPN and VPN protocols, we recommend using OpenVPN over Cloak from the first connection. If you use unmasked protocols, the ip of your VPS can be blocked.

Unmasked protocols OpenVPN over UDP, WireGuard and IKEv2 over UDP are easily detected by firewalls and some websites. Sites may show a warning: "disable VPN before visiting site".

To avoid this issue, use OpenVPN with the TCP protocol, OpenVPN over ShadowSocks, or OpenVPN over Cloak.

In all other cases, the difference between the protocols is minimal.
