## Sending files over a cellular phone circuit switched voice network connection?

- posted by: [goldenmean](https://stackexchange.com/users/-1/1120-goldenmean) on 2010-09-10
- tagged: `cellphone`
- score: 1

<p>I don't know if this would be off-topic here, but still asking.</p>

<ol>
<li><p>Does anyone has know of any technology for mobile phones that will allow to send large data files from one mobile phone to another distant mobile phone(Bluetooth is not the soln. for this), using just the receipeints mobile phone number, i.e. over the circuit switched voice network.(May be we can say an SMS with a attachment)</p></li>
<li><p>Would that kind of app. need a adaptation/support in the Protocol which GSM/CDMA (e.g. Push To Talk/Send applications) with support of Network side equipments able to support this feature as well as end user devices having this functionality. </p></li>
<li><p>This can be considered as Skype Send file equivalent, but difference being that this would be over a circuit switched point to point network flow without any internet connectivity needed for the two phones.</p></li>
</ol>

<p>Thank You and more if this doesn't get closed!</p>

<p>-AD</p>



## Answer 1806

- posted by: [Webs](https://stackexchange.com/users/-1/904-webs) on 2010-09-10
- score: 0

<p>To send files long distance you might be able to use bit torrent. I'm not sure anything exists to turn a smartphone into a torrent server, but it should be possible. Of course the data would still have to be sent as data traffic. See below for an explanation of this.</p>

<p>Why not use Dropbox or something like it to transfer files? Are you trying to avoid eating up your data bandwidth?</p>

<p>Sending files over voice would not be possible without some major hacking. The way communication works these days is you have all kinds of communication that takes place and those packets used for the communication are prioritized. With cell phones you have Voice, Data, and other for traffic as of right now I think. But at least Voice and Data for sure.</p>

<p>So without an app that can change the headers of packets to label them as voice (essentially tricking the networking equipment) so they get treated like voice packets, you will not be able to make this happen. Because anything that doesn't get dialed by the dialer on the phone, but still leaves the phone to communicate out is going to get marked by the router the phone communicates with as Data.</p>

<p>And once a carrier finds out you are doing this I would imagine they would try to shut down your app. Because your app would allow someone to get a very very basic plan and then have unlimited data over voice during nights and weekends. That would be a lot of lost profit for cell carriers.</p>




---

All content is licensed under [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/).
