# Unifi 

![Unifi Lineup](https://knowledge.9linedefense.com.us-southeast-1.linodeobjects.com/img/unifilineup.png)

## What is Unifi?

UniFi is Ubiquiti’s line of networking equipment with different models of wireless access points, routers, switches, cameras, and access control and many other products. UniFi equipment exists somewhere between enterprise and home networking appliances. It’s in the middle ground, offering more flexibility and features than most consumer-grade brands, but lacking the expense and complexity of enterprise grade equipment at a much higher price point. 

## Unifi Network Controller Software

The controller software is what ties all UniFi devices together, giving you a web interface so that you can manage and configure them. The controller software doesn’t need to be running all the time for the network to function correctly. It is only required to be running for configuration. Having the software running constantly has some pluses that are worth considering.

The software monitors and collects statistics about your network. UniFi devices don't have a lot of storage, and they require the controller software to log information about your network. Having it running all the time also saves you some configuration headaches, especially on a remote network. To get the full benefits of the UniFi ecosystem, **I recommend that you have an always-on controller.**

If you don’t want to run the UniFi Controller software, you can setup a UniFi access point in standalone mode using the mobile app. An AP in standalone mode is capable of providing Wi-Fi, but it’s other features are severely limited. Standalone APs can’t be managed remotely, and have a limited set of features.  I’d recommend running the UniFi Controller app somewhere to set up the access point rather than using standalone mode. Even if you turn off the controller when setup is over, the UniFi AP will be less limited and more useful. 

If you are not the server hosting type it is worth noting that the Unifi OS Consoles such as the Dream Machine and Cloud Keys can actually setup the controller for you locally. If you do not have one of those devices [HostiFi](https://www.hostifi.com/) is also a good SaaS Solution. 

## Unifi Equipment

(This image was provided from Evan McCann, I highly recommend you read his blog post on Unifi linked [here](https://evanmccann.net/blog/unifi-ecosystem-overview))

![UnifiEquipmentComparison](https://knowledge.9linedefense.com.us-southeast-1.linodeobjects.com/img/Unifi Equipment Comparison 2021.png)
![UnifiAPLineup](https://knowledge.9linedefense.com.us-southeast-1.linodeobjects.com/img/Unifi AP Lineup.png)