## Does the Sonos mesh network interfere with 802.11g or 802.11n?

- posted by: [Portman](https://stackexchange.com/users/-1/188-portman) on 2010-07-26
- tagged: `wifi`
- score: 3

<p><a href="http://www.sonos.com" rel="nofollow">Sonos</a> zone players and zone bridges create their own wireless <a href="http://en.wikipedia.org/wiki/Mesh_networking" rel="nofollow">mesh network</a> amongst one another. </p>

<p>Does this network use the same spectrum as Wifi (either "G" or "N")? And if so, is it possible that having Sonos devices in close proximity to your wifi access points is a bad idea?</p>



## Answer 737

- posted by: [Rich Seller](https://stackexchange.com/users/-1/68-rich-seller) on 2010-07-27
- score: 3

<p>Sonos <em>can</em> interfere with/be interfered with by WiFi if there are a lot of other networks nearby so there aren't any free channels. In this case you get contention on the network and data rates drop. If they drop below a certain point you'll experience issues because the data rate is no longer high enough for smooth playback. In practice this doesn't happen often as it is rare to get that many networks in close proximity, but it is worth bearing in mind if you see a lot of networks where you live.</p>

<p>An obvious alternative is to use wired Ethernet, or some HomePlug variant, instead of WiFi. I have Belkin's <a href="http://www.belkin.com/iwcatproductpage.process?product_id=495008" rel="nofollow">'Gigabit Powerline HD'</a> connecting two routers across my house and have had a good experience with it (the real data rate is around 100 Mbps but it is very stable)</p>

<p>Another thing to bear in mind is that other devices that use the same 2.4 GHz frequency can cause interference. For example <a href="https://sonos.custhelp.com/cgi-bin/sonos.cfg/php/enduser/std_adp.php?p_faqid=1063&amp;p_created=1270560832" rel="nofollow">Sonos recommend</a> you avoid using 2.4 GHz cordless phones near their equipment. Also beware of <a href="http://en.wikipedia.org/wiki/Electromagnetic_interference_at_2.4_GHz" rel="nofollow">possible interference</a> from video senders, baby monitors, older microwaves and even car alarms.</p>



## Answer 732

- posted by: [Joel Spolsky](https://stackexchange.com/users/-1/194-joel-spolsky) on 2010-07-27
- score: 1

<p>I have never seen a Sonos system interfere with WiFi... after all, WiFi itself doesn't interfere with WiFi (it's a protocol that allows multiple users on the same frequency). Sonos automatically picks a frequency to use, but you can override the channel, which I've found to be helpful in a larger system.</p>



## Answer 728

- posted by: [Scott A. Lawrence](https://stackexchange.com/users/-1/446-scott-a-lawrence) on 2010-07-26
- score: 0

<p>I thought their mesh network standard might be proprietary.  <a href="http://en.wikipedia.org/wiki/Sonos" rel="nofollow">This article</a> needs further verification, but I don't think standard wi-fi is affected.  <a href="http://www.joelonsoftware.com/items/2006/11/10.html" rel="nofollow">Joel Spolsky posted about Sonos</a> at some point in the past.  He mentions WiFi in the blog post multiple times, so it seems like there might be some connection.</p>




---

All content is licensed under [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/).
