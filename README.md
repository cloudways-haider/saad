[![Logo](http://i.imgur.com/Zd6tCxNh.png)](http://sipcapture.org)

#### 100% Open-Source VoIP Capture, Troubleshooting & Monitoring


![H5](https://img.shields.io/badge/HOMER-5-red.svg)
![HEP](https://img.shields.io/badge/proto-hep_eep-blue.svg)
![HEP](https://img.shields.io/badge/proto-sip-brightgreen.svg)
![HEP](https://img.shields.io/badge/proto-rtcp-brightgreen.svg)
![HEP](https://img.shields.io/badge/proto-rtcp_xr-brightgreen.svg)
![HEP](https://img.shields.io/badge/proto-rtp_stats-brightgreen.svg)
![HEP](https://img.shields.io/badge/text-QoS-green.svg)
![HEP](https://img.shields.io/badge/text-syslog-green.svg)
![HEP](https://img.shields.io/badge/text-CDRs-green.svg)


<img src="http://i.imgur.com/9AN08au.gif" width=100% height=50 >


## What is HOMER?

**HOMER** is a robust, carrier-grade, scalable SIP Capture system and VoiP Monitoring Application offering [HEP/EEP](http://github.com/sipcapture/hep), IP Proto4 (IPIP) encapsulation & port mirroring/monitoring support right out of the box, ready to process & store insane amounts of signaling, logs and statistics with instant search, end-to-end analysis and drill-down capabilities for ITSPs, VoIP Providers and Trunk Suppliers using SIP signaling protocol.

Powered at the core by [SIPCAPTURE](http://kamailio.org/docs/modules/stable/modules/sipcapture.html) Module for industry-standard [Kamailio](http://kamailio.org) or [OpenSIPS](http://opensips.org), HOMER provides virtually unlimited scope for granular capture [configuration](https://github.com/sipcapture/homer-api/blob/master/examples/sipcapture/kamailio.cfg) either stand-alone or using our companion [Capture Agent](https://github.com/sipcapture/captagent) Project.

**HOMER 5** User-Interface is developed using standard Angular JS, easily extensible and with all functionality moved to specialized and customizable widgets feeding and displaying correlated data from internal and external data sources such as InfluxDB and Elasticsearch. 

**HOMER** allows integrators and users to define granular custom logic and generate statistic from its capture dialplan interacting with other Kamailio modules to extend its functionality including fully programmable threshold triggering and alarming, providing plenty of space for tailored configurations and logic customizations.

**HOMER** is already used by large voice networks, voip service providers and traffic carriers worldwide, has been implemented as a service in 3rd party voice platforms and is suitable for production. Contact the team for your basic and advanced needs or leverage the experience of our great community by joining our [mailing-list](http://groups.google.com/group/homer-discuss). 

<br/>

## Installation & Configuration

Please follow our [Wiki](https://github.com/sipcapture/homer/wiki) and learn how to [setup](https://github.com/sipcapture/homer/wiki/Quick-Install) and [use](https://github.com/sipcapture/homer/wiki/Using-Homer-5) HOMER, configure [capture agents](https://github.com/sipcapture/homer/wiki/Examples%3A-Captagent4) _([Kamailio](https://github.com/sipcapture/homer/wiki/Examples%3A-Kamailio), [OpenSIPS](https://github.com/sipcapture/homer/wiki/Examples%3A-OpenSIPS), [Asterisk](https://github.com/sipcapture/homer/wiki/Examples%3A-Asterisk), [FreeSwitch](https://github.com/sipcapture/homer/wiki/Examples%3A-FreeSwitch), [sipgrep](https://github.com/sipcapture/homer/wiki/Examples%3A-sipgrep), [sngrep](https://github.com/sipcapture/homer/wiki/Examples%3A-sngrep))_, ship [custom logs](https://github.com/sipcapture/homer/wiki/Examples%3A-hepipe.js), custom [statistics](https://github.com/sipcapture/homer/wiki/Example%3A-CustomStats), create [encrypted HEP tunnels](https://github.com/sipcapture/homer/wiki/hepstunnel) and much more.


<img src="http://i.imgur.com/DdnUXe6.gif" />


### Need Support?
For professional support, remote installations, customizations or commercial requests please contact: support@sipcapture.org

For community support, updates, user discussion and experience exchange please join our users   [Mailing-List](https://groups.google.com/forum/#!forum/homer-discuss)


[![Join the chat at https://gitter.im/sipcapture/homer](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/sipcapture/homer?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)


<img src="http://i.imgur.com/9AN08au.gif" width=100% height=50 >

# HOMER Components

<img src="http://i.imgur.com/0qiWlzi.png" >


## Capture Server <a href="http://github.com/sipcapture/HEP"><img src="http://i.imgur.com/RSUlFRa.gif"></a>

Responsible for Collecting, Indexing and Storing received HEP, IPIP and Raw packets from HEP Agents, the HOMER Capture Server is based on our SIPCapture module for [Kamailio](http://kamailio.org) or [OpenSIPS](http://opensips.org) featuring optimized database schemas with advanced options and complex and extensible capture plans with multiple table support and triggers able to interact with any module on the platform and unlimited scope. Includes a powerful and modern [Web User-Interface](https://github.com/sipcapture/homer-ui) and secure [REST API](https://github.com/sipcapture/homer-api)

<img src="http://i.imgur.com/p9wV9kh.png">

## Capture Agents <a href="http://github.com/sipcapture/HEP"><img src="http://i.imgur.com/RSUlFRa.gif"></a>

Capture Agents are responsible for feeding HOMER [SIP signaling](https://github.com/sipcapture/homer/wiki), [Logs](https://github.com/sipcapture/homer/wiki/Examples%3A-hepipe.js), [RTP/RTCP Reports](https://github.com/sipcapture/homer/wiki/Using-Homer-5-QoS-Reports), [Custom Statistics](https://github.com/sipcapture/homer/wiki/Example%3A-CustomStats) and much more using the HEP _(Homer Encapsulation Protocol)_ protocol. Our [WIKI](https://github.com/sipcapture/homer/wiki) provides several useful examples to get started.

The following projects are _HEP-ready_:

* [Kamailio](https://github.com/sipcapture/homer/wiki/Examples%3A-Kamailio)
* [OpenSIPS](https://github.com/sipcapture/homer/wiki/Examples%3A-OpenSIPS)
* [Asterisk](https://github.com/sipcapture/homer/wiki/Examples%3A-Asterisk)
* [FreeSWITCH](https://github.com/sipcapture/homer/wiki/Examples%3A-FreeSwitch)
* [RTPEngine](https://github.com/sipcapture/homer/wiki/Examples%3A-RTPEngine) 
* [sngrep](https://github.com/sipcapture/homer/wiki/Examples%3A-sngrep)
* [sipgrep](https://github.com/sipcapture/homer/wiki/Examples%3A-sipgrep)
+ [CaptAgent](http://github.com/sipcapture/captagent) _for any other platform_



<img src="http://i.imgur.com/9AN08au.gif" width=100% height=50 >







##### HOMER's [Captagent](http://github.com/sipcapture/captagent) is now also available on [Github](http://github.com/sipcapture/captagent)

### Developers
Contributors and Contributions to our project are always welcome! If you intend to participate and help us improve HOMER by sending patches, we kindly ask you to sign a standard [CLA (Contributor License Agreement)](http://cla.qxip.net) which enables us to distribute your code alongside the project without restrictions present or future. It doesn’t require you to assign to us any copyright you have, the ownership of which remains in full with you. Developers can coordinate with the existing team via the [homer-dev](http://groups.google.com/group/homer-dev) mailing list. If you'd like to join our internal team and volounteer to help with the project's many needs, feel free to contact us anytime!




### License & Copyright

![H5](https://img.shields.io/badge/license-GNU_AGPL_v3-blue.svg)

Homer components are released under the GNU Affero General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

*(C) 2008-2016 [SIPCAPTURE](http://sipcapture.org) & [QXIP BV](http://qxip.net)*

----------

##### If you use HOMER in production, please consider supporting the project with a [Donation](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=donation%40sipcapture%2eorg&lc=US&item_name=SIPCAPTURE&no_note=0&currency_code=EUR&bn=PP%2dDonationsBF%3abtn_donateCC_LG%2egif%3aNonHostedGuest)

[![Donate](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=donation%40sipcapture%2eorg&lc=US&item_name=SIPCAPTURE&no_note=0&currency_code=EUR&bn=PP%2dDonationsBF%3abtn_donateCC_LG%2egif%3aNonHostedGuest) 

# saad
# saad
