## How long does a SIM card last?

- posted by: [gyurisc](https://stackexchange.com/users/-1/143-gyurisc) on 2010-07-15
- tagged: `cellphone`, `mobile-phones`, `sim-card`
- score: 4

<p>Today I called my cell phone operator and asked them what the expected lifetime of a SIM card is. They couldn't say anything except that a SIM card can get demagnetized at any time.</p>

<p>Well, I know that any electronic device can break at any time, thank you. And I know that a SIM card doesn't use anything like magnetic strip, so it just breaks, not "gets demagnetized".</p>

<p>What's the expected lifetime of a SIM card? Are there any specs/manufacturer claims/standards?</p>



## Answer 245

- posted by: [DougC](https://stackexchange.com/users/-1/88-dougc) on 2010-07-15
- score: 9

<p>I think your phone company has no idea (no surprise there). The SIM card contains a chip which is powered and read via the metal pads on the side. Although in theory there probably is a finite lifetime to it, it is in practice an extremely simple thing and I suspect that, treated well, will outlive its owner. I have had one of my phones for probably 10 years at least and transferred it between 4 or 5 phones and it still works fine. That also includes transferring it into other devices temporarily on maybe a dozen occasions.</p>



## Answer 285

- posted by: [geoffc](https://stackexchange.com/users/-1/13-geoffc) on 2010-07-15
- score: 2

<p>The gold contacts on the SIM card are the I/O ports for a special purpose CPU, with RAM.  Depending on the SIM, it is usually on the order of a 32 Mhz CPU, with 128K of RAM.  This is optimized to generate RSA key pairs.  </p>

<p>This is basically a digital certificate stored on a card, like the bigger Smart Cards, with a little bit of extra storage.  It uniquely identifies the card to the cellular network, in a way that is hard (currently considered impossible, but that could change) to fake. </p>

<p>So the contacts could wear out from sliding in and out, (unlikely) but it is hard to imagine the CPU/RAM having an issue due to age, anymore than modern CPUs.  The core difference between a computer CPU and a SIM would be the amount of heat generated.  The modern CPU is in use all the time.  The SIM CPU is used to generate new certs and to sign authorization requests to the network.  </p>

<p>Personally I have had bizarre SIM issues on TMobile though.  They claimed my 18 month old SIM was the cause of my flaky phone service.  So I switched it.  No appreciable change.   (BB 8320 Curve).</p>

<p>Switched to a BB 9700 Bold, same SIM, could not get 3G coverage, even in the heart of NYC.  They said, oh it must be the SIM, which I thought was utter nonsense as it was only 3 months old.  But lo and behold, I switched SIMs and suddenly I was getting 3G everywhere I went.   (Well everywhere that TMobile's fairly lousy 3G coverage extends). </p>




---

All content is licensed under [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/).
