## Phones for java development

- posted by: [Eric](https://stackexchange.com/users/-1/990-eric) on 2010-08-24
- tagged: `mobile-phones`, `java`, `development`
- score: 1

<p>I'm searching for a new phone, after my last one (a samsung J700) was lost to a tragic incident involving a washing machine and dryer.</p>

<p>Ideally, I'd like to be able to write java applets, and run them on my new (currently) unbought phone. However, no phone vendors seem to be very good at specifying java support.</p>

<p>Is there a master list somewhere of all phones that support Java development?</p>



## Answer 1556

- posted by: [Webs](https://stackexchange.com/users/-1/904-webs) on 2010-08-24
- score: 1

<p>[UPDATE]:
Have you looked into the Nokia phones, the ones that aren't Android based. I'm pretty sure they ran some variant of Linux and were supposedly more open than Android phones. Also you could try OpenMoko. If OpenMoko doesn't support it probably no phone will. But if OpenMoko doesn't support it there is also a chance you could get a java compiler to work on it. OpenMoko is *.nix based.</p>

<p>[ORIGINAL]:</p>

<p>For Android I think I <a href="http://javathings.blogspot.com/2009/03/java-applications-j2me-on-android.html" rel="nofollow">found your answer here</a>:</p>

<blockquote>
  <p>Android does not support J2ME out of
  the box. Strictly speaking, you will
  not be able to run Java applications
  written for other mobile platforms
  (devices not based on Android).</p>
  
  <p>Android is basically an alternative to
  J2ME, a rewrite. Most people seem to
  agree that Android is much more
  powerful alternative. Android already
  has a more active community and there
  is already a lot of useful libraries
  incorporated in it, which are missing
  from J2ME.</p>
  
  <p>So if you have a J2ME application that
  you want to run on Android device, you
  want to port the code to make best use
  of Android API features and achieve
  best performance.</p>
  
  <p>Alternatively you can look into "J2ME
  for Android" adapters written by
  someone else. Not sure if there is any
  production quality adapters out there
  or if Google will ever create a decent
  adapter or emulator for J2ME
  applications.</p>
</blockquote>

<p>One such tool you can try is called J2Android.</p>

<p>For other phones I think support is just as sparing.</p>



## Answer 1603

- posted by: [Peter Mortensen](https://stackexchange.com/users/-1/118-peter-mortensen) on 2010-08-27
- score: 0

<p>The Nokia phones with <a href="http://en.wikipedia.org/wiki/Series_40" rel="nofollow">Series 40</a> can run Java applets.</p>

<p>That referenced page contains 177 Series 40 Nokia phone models: </p>

<blockquote>
  <p>1680, 2220, 2320, 2323, 2330, 2355, 2600, 2610, 2626, 2630, 2650, 2660, 2680, 2690, 2700, 2710, 2720, 2730, 2760, 2855, 2865, 2865, 3100, 3105, 3108, 3109, 3110, 3110, 3120, 3120, 3125, 3152, 3155, 3155, 3200, 3205, 3220, 3280, 3300, 3300, 3500, 3510, 3530, 3555, 3585, 3586, 3586, 3587, 3587, 3595, 3600, 3610, 3710, 3720, 5000, 5070, 5100, 5130, 5140, 5140, 5200, 5220, 5300, 5310, 5330, 5610, 6010, 6012, 6015, 6015, 6020, 6030, 6060, 6070, 6080, 6085, 6086, 6100, 6101, 6102, 6102, 6103, 6108, 6111, 6125, 6126, 6131, 6131, 6133, 6136, 6151, 6152, 6155, 6155, 6165, 6170, 6200, 6208, 6212, 6216, 6220, 6225, 6230, 6230, 6233, 6234, 6235, 6235, 6255, 6260, 6263, 6265, 6265, 6267, 6270, 6275, 6275, 6280, 6282, 6288, 6300, 6300, 6301, 6303, 6260, 6500, 6500, 6555, 6585, 6600, 6600, 6600, 6610, 6610, 6650, 6651, 6700, 6750, 6800, 6800, 6810, 6820, 6822, 7020, 7070, 7100, 7200, 7210, 7210, 7230, 7250, 7250, 7260, 7270, 7310, 7360, 7370, 7373, 7390, 7500, 7510, 7600, 7610, 7900, 8600, 8800, 8800, 8800, 8800, 8800, 8801, 8910i, X2, X3, C3, and X3-02.</p>
</blockquote>

<p>It is not easy to find a place to start from in order to write Java applets, but I believe the central place for Nokia Series 40 is: <a href="http://www.forum.nokia.com/Develop/Java/" rel="nofollow">http://www.forum.nokia.com/Develop/Java</a>/</p>



## Answer 1612

- posted by: [Dan Dyer](https://stackexchange.com/users/-1/916-dan-dyer) on 2010-08-28
- score: 0

<p>Applets, in Java terminology at least, are a (browser-based) desktop technology.  For phone development, assuming you mean JavaME, you would be writing MIDlets, which are considerably more constrained in what they can do.  There are also various JavaME profiles and JSRs meaning that different devices have different capabilities.  However, anything that runs Symbian Series 40 or Series 60 should have some level of JavaME support.</p>

<p>The Android platform is much closer to desktop Java than JavaME is and, so far, not nearly as fragmented.</p>




---

All content is licensed under [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/).
