## How secure is using only MAC ID Filtering as compared to other WiFi security methods?

- posted by: [just mike](https://stackexchange.com/users/-1/319-just-mike) on 2010-07-27
- tagged: `wifi`, `security`
- score: 1

<p>If I set up a WiFi router to only allow in those MAC addresses that I specify, and use no other security methods, how secure is the router and network compared to using other security methods?</p>



## Answer 754

- posted by: [joyjit](https://stackexchange.com/users/-1/353-joyjit) on 2010-07-27
- score: 6

<p>It is insecure compared to, say WPA (with password). It is relatively easy to spoof MAC addresses. So a malicious user, by spoofing a valid MAC address, could get into your network.</p>



## Answer 762

- posted by: [firedfly](https://stackexchange.com/users/-1/10-firedfly) on 2010-07-27
- score: 6

<p>If you only use MAC address filtering, a large portion of the network traffic going across the wireless network will be unencrypted--it would be up to each application to encrypt the traffic.  This would allow someone to listen to the traffic on your wireless network and see what data is being transferred.  The user would not need to spoof the MAC address and join the network to see the data.  They would just need to listen to the traffic broadcast on the network.</p>

<p>I would recommend some kind of encryption on the network.  Unless things have changed in the last few years, I'd stay away from WEP as well.</p>




---

All content is licensed under [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/).
