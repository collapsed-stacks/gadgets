## Why do smartphones need an internet connection to acquire a GPS position?

- posted by: [badp](https://stackexchange.com/users/-1/1089-badp) on 2010-09-06
- tagged: `gps`
- score: 3

<p>I am the owner of a dedicated GPS receiver (a small box with just a on/off switch and a bluetooth link) and a (lowish end) smartphone with an integrated GPS receiver.</p>

<p>One'd think that the processing power of a smartphone could run laps around the dedicated receiver's.</p>

<p>Somehow, however, the dedicated receiver can triangulate my position without "external help", while the smartphone basically requires an internet connection to do the same in a timely manner.</p>

<p>Why is that?</p>



## Answer 1747

- posted by: [GAThrawn](https://stackexchange.com/users/-1/171-gathrawn) on 2010-09-06
- score: 8

<p>The important point with GPS speed is "<a href="http://en.wikipedia.org/wiki/Time_to_first_fix" rel="nofollow">time to first fix</a>", this is the time it takes the GPS device to work out where you are in the world from when it is switched on to when it has an accurate fix.</p>

<p>Old-fashioned GPS devices used to take a long time (over 10-15 minutes in many cases) to calculate to calculate this from "cold" (ie when they've been switched off for a while) this was taken up with detecting the signals from multiple satellites, waiting for then downloading the satellite position and timing data, and putting this all together to get a fix. Over time manufacturers worked out that they could do shortcuts like saving the satellite data, and then saving the last known time and position in the device's memory,  and then compare the signals received with that to speed things up. This has the drawback that it only speeds things up if you're in roughly the same part of the world as when you last switched it on, but you do at least have the satellite data so don't have to wait around for that.</p>

<p>Smartphones often use a shortcut to get the first fix, where they'll use some other method to get your rough location. Typically either by identifying which cell towers are in range, and then looking these up over the internet on a database of known cell tower positions, or by scanning for WiFi networks in the area, and looking the SSIDs of these up ona database over the internet. It's this step of identifying cell phone towers or WiFi that needs the internet connection to connect to the database that matches the ID to a physical location.</p>

<p>The advantage that standalone GPS receivers have is that all their hardware and software is dedicated to and optimised for GPS use, they have just one radio antenna, that can be as big as needed to receive weaker signals, they have just one signal processor that is optimised to process GPS signals, their software is optimised for just getting GPS fixes and displaying maps. This means that the GPS device should be able to pick up weaker signals, so be able to see more satellites, so get a faster fix with less assistance.</p>

<p>Whereas on a smartphone the GPS is a second-class citizen forced to work alongside a whole load of other gear. Typical phones need to pick up (and transmit) radio signals for GSM, GPRS, HSDPA/3G, Bluetooth, FM Radio, WiFi and GPS. There will be multiple radio antennas for these (of which the ones for voice and data will be probably be given the favoured locations and space) and the software is more general purpose, and any tuning and optimising will be aligned to voice and data, as they're the ones people really complain about when their signal gets dropped. What this adds up to is that the GPS antenna in a phone can normally only pick up stronger signals, not weak ones, so sees less satellites at one time, so needs more help to get a fast fix.</p>



## Answer 1749

- posted by: [Dennis Williamson](https://stackexchange.com/users/-1/89-dennis-williamson) on 2010-09-06
- score: 0

<p>Dedicated GPS units carry their maps on board. Smartphones often retrieve their maps on the fly.</p>




---

All content is licensed under [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/).
