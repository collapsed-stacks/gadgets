## Updating a BB to new OS

- posted by: [geoffc](https://stackexchange.com/users/-1/13-geoffc) on 2010-08-11
- tagged: `blackberry`, `os-update`
- score: 0

<p>Now that the BB Torch with OS 6 is released, I just got my BB desktop software update notice, and am updating.  </p>

<p>I am on TMobile with a BB 9700 Bold and they seem to be notoriously slow on allowing updates.</p>

<p>Is there a 1) legal, and 2) safe way to get the upgrade onto my phone?</p>



## Answer 1278

- posted by: [GAThrawn](https://stackexchange.com/users/-1/171-gathrawn) on 2010-08-11
- score: 2

<p>I've updated my BB's software lots of times with no problems. It is definitely worth using the Desktop Manager's Backup function to do a full backup of you data and apps before starting though.</p>

<p>Go to the handheld software downloads page <a href="http://na.blackberry.com/eng/support/downloads/download_sites.jsp" rel="nofollow">http://na.blackberry.com/eng/support/downloads/download_sites.jsp</a> find your country and service provider, then select your phone model and it should take you straight to a list of firmware updates that your network has authorised.</p>

<p>If there is a newer update for your model in the list, just download it, then run the EXE. Once it's installed, start up Blackberry Desktop Manager and plug in your Blackberry, you should be prompted to upgrade and from now on it walks you through a simple wizard.</p>

<p>Alternatively <em>(and this is the method that won't be supported by your phone company, but shouldn't invalidate your hardware warranty with RIM as you're still using software supplied by them)</em> browse through other phone networks that use the same technology (GSM/CDMA) and frequencies as yours <em>(that bit is important, you need to make sure the update is for the exact same hardware as yours, otherwise you can break your phone)</em> and see if they have the update for your BB. If they do, download it and install it. Once installed on your pc explore to c:\Program Files\Common Files\Research In Motion\AppLoader and then delete the Vendor.xml file, this is the file that specifies which networks that upgrade can be used on. Now plug-in your Blackberry and continue the upgrade as above.</p>




---

All content is licensed under [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/).
