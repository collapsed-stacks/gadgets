## Home Automation

- posted by: [EricR](https://stackexchange.com/users/-1/274-ericr) on 2010-07-22
- tagged: `wifi`, `accessories`, `home-automation`
- score: 3

<p><strong>It was suggested that I migrate <a href="http://serverfault.com/questions/162073/home-automation-closed">this question</a> here, from serverfault.</strong></p>

<p>I was reading about home automation on wikipedia a little, couldn't find a foot hold.</p>

<p><a href="http://en.wikipedia.org/wiki/Category:Home_automation" rel="nofollow">http://en.wikipedia.org/wiki/Category:Home_automation</a></p>

<p>I was wondering what your opinions were on home automation, e.g., ethernet coffee pot, control of temperature, sensors for reading in data like temperature, power usage, etc. 
At least as far as feasibility for a home project, sensors throughout the house, video etc., all linked back to a central home server. What are good companies for purchasing remotely controlled power/devices, especially ones I could interact with through linux.</p>



## Answer 564

- posted by: [KeithB](https://stackexchange.com/users/-1/199-keithb) on 2010-07-22
- score: 4

<p>I have a bunch of Insteon devices throughout my house.  Mostly switches, but I've played with some motion sensors, timers, and and IR-Insteon bridge.  You need a bit of electrical knowledge (or pay someone to do it) to replace the switches, especially multi-way switches. Its great for controlling lights from places that they weren't wired for.  As an example, we have outside spotlights at the front and back of the house.  I set it up so that the original switches control both sets, and they can also be controlled from the bedroom.</p>

<p>Insteon is an updated version of the old X10 protocol, that is much more reliable.  It sends its signals over your houses existing wiring. I haven't had any issues with commands not going through.  A good place to start is <a href="http://smarthome.com" rel="nofollow">Smart Home</a> and <a href="http://machomestore.com" rel="nofollow">Mac Home Store</a></p>



## Answer 553

- posted by: [Rich Seller](https://stackexchange.com/users/-1/68-rich-seller) on 2010-07-22
- score: 3

<p>Have a look at <a href="http://www.insteon.net/" rel="nofollow">Insteon</a>. It has modules for all kinds of things including <a href="http://www.insteon.net/31279-EZSrve.html" rel="nofollow">ethernet</a>, <a href="http://www.insteon.net/HVAC.html" rel="nofollow">HVAC</a>, <a href="http://www.insteon.net/2413S-powerlinc-dual-band.html" rel="nofollow">power control</a> and supports PC interaction (<a href="http://www.linuxha.com/athome/common/iplcd/" rel="nofollow">including Linux</a>) and can be controlled with <a href="http://www.insteon.net/handheld-remotes.html" rel="nofollow">dedicated remotes</a> or even be controlled with an <a href="http://gadgets.stackexchange.com/questions/39" rel="nofollow">iPhone</a>.</p>



## Answer 847

- posted by: [Portman](https://stackexchange.com/users/-1/188-portman) on 2010-07-29
- score: 2

<p>Also take a look at Control4 (<a href="http://www.control4.com/" rel="nofollow">corporate website</a> or <a href="http://en.wikipedia.org/wiki/Control4" rel="nofollow">wikipedia</a>). Although Control4 is a proprietary brand, it uses the relatively new <a href="http://en.wikipedia.org/wiki/Zigbee" rel="nofollow">802.15.4 "ZigBee" protocol</a>. Everything is strictly IP-based, making it very easy for software developers to write their own controllers.</p>

<p>I don't have any personal experience with Control4, but I've been looking to upgrade my aging X10 devices for a while and if I had to commit today I would probably pick Control4.</p>




---

All content is licensed under [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/).
