## How to overclock Nokia N900?

- posted by: [silvo](https://stackexchange.com/users/-1/440-silvo) on 2010-07-28
- tagged: `mobile-phones`
- score: 1

<p>My Nokia N900 is becoming slower and slower. Sometimes it is so bad that I have to wait up to 10 seconds for a new browser tab to open or cannot watch a divx movie due to stuttering. Did anyone try to overclock N900? Is it safe? How much of a difference did it make?</p>



## Answer 851

- posted by: [bongster](https://stackexchange.com/users/-1/508-bongster) on 2010-07-29
- score: 2

<p>There is a reason Nokia decided to set the max. clock frequency to what they have chose.
Overclocking is dangerous: depending on which side/corner of the wafer the actual silicon for the N900's CPU chip came from -- your overclocking may or may not actually work.</p>

<p>It will most certainly void your warranty.</p>

<p>It will probably also reduce the overall life of your device (caused by overheating)</p>

<p>In spite of all these warnings, if you do decide to go for it, <a href="http://themeegoblog.com/2010/04/04/how-to-overclock-the-nokia-n900/" rel="nofollow"><strong>here is a great tutorial on how to do it</strong></a>.</p>



## Answer 845

- posted by: [njd](https://stackexchange.com/users/-1/201-njd) on 2010-07-29
- score: 0

<p>Assuming you <em>could</em> overclock it, the extra heat might cause problems, and you'd probably drain the battery much faster.<br>
Apparently <a href="http://talk.maemo.org/showthread.php?t=42960&amp;page=10" rel="nofollow">someone has</a> overclocked their N900, but it only resulted in more movie stuttering.</p>

<p>It might be safer to try to find out what software issue is causing the slowdown before you try messing with the hardware.  </p>

<p>Are you running an especially busy theme? Have you cleared out the browser cache recently?</p>

<p>This <a href="http://talk.maemo.org/showthread.php?t=43429" rel="nofollow">link</a> has a few suggestions, like running <code>top</code> in a terminal to find out what's hogging the CPU. (Here's a <a href="http://talk.maemo.org/showpost.php?p=505549&amp;postcount=30" rel="nofollow">pic</a> of <code>top</code> running on the N900)</p>

<p>Also <a href="http://talk.maemo.org/showthread.php?t=42960" rel="nofollow">this thread</a> has suggestions like running in a terminal:</p>

<pre><code>df -h|grep rootfs
</code></pre>

<p>to see if the filesystem is getting too full.</p>




---

All content is licensed under [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/).
