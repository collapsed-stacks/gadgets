## Downgrade Sansa Fuze firmware to install Rockbox

- posted by: [Broam](https://stackexchange.com/users/-1/185-broam) on 2010-07-16
- tagged: `firmware`, `rockbox`, `sansa`
- score: 0

<p>I've read on the Rockbox website that only specific versions of Sansa Fuze firmware are supported. Is it possible to downgrade my Fuze to an older firmware in order to facilitate the install?</p>

<p>My Fuze v2 is running 2.02.33, whereas Rockbox wants 2.02.26.</p>



## Answer 453

- posted by: [Broam](https://stackexchange.com/users/-1/185-broam) on 2010-07-19
- score: 1

<p>The Rockbox team generally find out how to patch the latest firmware versions, given enough time; there's a delay of course.</p>

<p>Conjecture would state that they do this so that if Sansa retracts old firmware versions the new ones will also work (and also to assist users if the Fuze is unable to be downgraded.)</p>

<p>tldr: <strong>2.02.33 is able to be patched.</strong> I've installed using it.</p>



## Answer 452

- posted by: [njd](https://stackexchange.com/users/-1/201-njd) on 2010-07-19
- score: 0

<p>I've done this with a Clip and Clip+, so I'd expect the same thing to work with a Fuze.</p>

<p>The <a href="http://forums.sandisk.com/sansa/board?board.id=sansafuse" rel="nofollow">Sansa Forums</a> are a good source of information on firmware versions.</p>

<p>Try downloading 2.02.26 from <a href="http://mp3support.sandisk.com/firmware/fuze/fuze02.02.26.zip" rel="nofollow">this link</a> and extract the <code>fuzpa.bin</code></p>

<p>You should be able to use the Rockbox Utility to apply the firmware (though I confess I've only used it with a Clip/Clip+, not a Fuze).</p>

<p>When you install the bootloader, RockboxUtility asks you for the firmware, and you can pass it the fuzpa.bin you just extracted from the fuze02.02.26 zip file.
RockboxUtility takes care of applying the Sansa firmware.</p>




---

All content is licensed under [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/).
