## Good and cheap Car Fleet Alarm system

- posted by: [adopilot](https://stackexchange.com/users/-1/583-adopilot) on 2010-07-31
- tagged: `gps`, `alarm`, `gps-tracking`
- score: 1

<p>Any recommendation for Car GPS tracking security device.<br>
What I will love to avoid is monthly fee for Server.<br>
I just want to be able to find coordinates of my vehicle  by 3G if it is posibile if not by SMS.</p>



## Answer 958

- posted by: [Rich Seller](https://stackexchange.com/users/-1/68-rich-seller) on 2010-07-31
- score: 2

<p>You could do this with an android phone and the <a href="http://tasker.dinglisch.net/" rel="nofollow">Tasker</a> app. It can be configured to periodically enable GPS to get the current location then send that location as an SMS or HTTP update. Of course this means you need a functioning phone in each vehicle but you would probably want that anyway. The phone need not be that advanced, it would just need to be running a recent version of Android and have GPS. The Tasker app only costs a few dollars.</p>

<p><strong>Update:</strong> Here is a set of Tasker profiles that allow for an intermittent update of the handset's location. It needs two profiles because currently Tasker doesn't have a "get location fix" type call, so this can be achieved instead by activating a location-based profile. </p>

<p><em>Note that this profile works for me, but I'm quite new to Tasker so it may not be the optimal approach. If anyone knows a better way to do any part of it then please comment on this answer.</em></p>

<p>The first profile is location based and gets the GPS fix. The second profile is timer based and activates the first, then waits for a while before posting the details.</p>

<p>To create the first profile open Tasker and:</p>

<ul>
<li>At the main menu select <strong>New</strong>-><strong>Location</strong>, then <strong>Done</strong>.</li>
<li>At the <strong>Name Context</strong> dialog, enter <strong>Location</strong>, then press <strong>OK*</strong>.</li>
<li>At the <strong>Task Edit</strong> screen, select the <strong>+</strong> icon, then <strong>Variable</strong> then <strong>Variable Set</strong>.</li>
<li>In the <strong>Variable Set</strong> screen, set <strong>Name</strong>=**%LOC_TIMESTAMP** and <strong>To</strong> to <strong>%DATE</strong>, then press <strong>Done</strong>.</li>
<li>Press <strong>Done</strong> again to return to the main Tasker screen.</li>
<li>We actually want the LOC_TIMESTAMPto be set when the profile exits, so tap on the <strong>Variable Set ...</strong> item on the right and select <strong>Move To Exit</strong> to make it an exit event.</li>
<li>We don't want this profile to be active, so tap on the <strong>Location</strong> flag, then in the <strong>Context Options</strong> dialog, select <strong>Profile</strong> then <strong>Disable</strong>.</li>
<li>The profile needs to have a name to be used by other profiles, so long-tap on the profile's header bar then in the <strong>Profile Options</strong> dialog, select <strong>Name</strong>, then in the <strong>Name Profile</strong> dialog enter <strong>Current Location</strong>.</li>
</ul>

<p>You now have a profile that will get a location fix when activated and set the LOC_TIMESTAMP variable to the date when the profile was deactivated. This gives a pretty accurate record of the last location fix.</p>

<p>We now need another profile to periodically activate the <strong>Current Location</strong> profile and send the data somewhere:</p>

<ul>
<li>From the main Tasker screen, select <strong>New</strong>-><strong>Time</strong>.</li>
<li>In the dialog set <strong>From:</strong> to <strong>9:00</strong> and To: to <strong>17:00</strong> (assuming you only want to track 9-5, if you want to have this active constantly, uncheck both the <strong>From:</strong> and <strong>To:</strong> fields). Check <strong>Repeat:</strong> and set the value to <strong>30 Minute(s)</strong>.</li>
<li>In the <strong>Task Edit:</strong> screen we need to add 3 tasks:
<ul>
<li>First make note of the current GPS status so we can turn it off when done if needed:
<ul>
<li>Select <strong>+</strong>-><strong>Variable</strong>-><strong>Variable Set</strong>.</li>
<li>Set <strong>Name</strong> to <strong>%WASGPS</strong> and <strong>To</strong> to <strong>%GPS%</strong>.</li>
<li>Select Done.</li>
</ul></li>
<li>Second turn GPS on if it is off:
<ul>
<li>Select <strong>+</strong>-><strong>Misc</strong>-><strong>GPS</strong>.</li>
<li>In the <strong>GPS</strong> dialog set <strong>Set</strong> to <strong>On</strong>.</li>
<li>Check <strong>If</strong> then in the three fields enter the respective values <strong>%WASGPS</strong>, <strong>~</strong> (equals), and <strong>Off</strong></li>
<li>Select <strong>Done</strong>.</li>
</ul></li>
<li>Third enable the <strong>Current Location</strong> profile:
<ul>
<li>Select <strong>+</strong>-><strong>Tasker</strong>-><strong>Profile Status</strong>.</li>
<li>In the <strong>Profile Status</strong> dialog, long-click in the <strong>Name</strong> field, select the <strong>Current Location</strong> profile from the <strong>Select Profile</strong> list (this is why it needs to be named).</li>
<li>Set the <strong>Set</strong> field to <strong>On</strong>.</li>
<li>Select <strong>Done</strong>.</li>
</ul></li>
</ul></li>
<li>Select <strong>Done</strong> to return to the main Tasker screen.</li>
</ul>

<p>We now need to add some exit actions to the new profile. We need to configure the exit tasks to wait for enough time for a GPS fix to be established (at least I think we do, you may be able to omit this step), then turn the location profile off, disable GPS, and send the location notification.</p>

<ul>
<li>Tap on the right hand side of the new profile and select <strong>Add Exit Task</strong>.
<ul>
<li>First wait for a minute:
<ul>
<li>Select <strong>+</strong>-><strong>Tasker</strong>-><strong>Wait</strong>.</li>
<li>In the <strong>Wait</strong> dialog, set <strong>Minutes</strong> to <strong>1</strong>.</li>
<li>Select Done.</li>
</ul></li>
<li>Deactivate the <strong>Current Location</strong> profile. Steps are the same as above, but set <strong>Set</strong> to <strong>Off</strong>.</li>
<li>Deactivate GPS if it wasn't active before the task ran.
<ul>
<li>Select <strong>+</strong>-><strong>Misc</strong>-><strong>GPS</strong></li>
<li>In the <strong>GPS</strong> dialog set <strong>Set</strong> to <strong>Off</strong>.</li>
<li>Check <strong>If</strong> then in the fields enter <strong>%WASGPS</strong>, <strong>~</strong> (equals), and <strong>On</strong></li>
<li>Select <strong>Done</strong>.</li>
</ul></li>
<li>Notify the current position. You can do this by sending an SMS or by sending an HTTP Post to a web service if you like. There is also an option to compose an email, but I don't see an automatic way of actually sending one. To send an SMS:
<ul>
<li>Select <strong>+</strong>-><strong>Phone</strong>-><strong>Send SMS</strong>.</li>
<li>Long-click the <strong>Number</strong> field and pick a contact to spam.</li>
<li>In the <strong>Message</strong> field, enter <strong>%LOC_TIMESTAMP: %LOC</strong>.</li>
<li>Select <strong>Done</strong>.</li>
</ul></li>
<li>To send an HTTP Post:
<ul>
<li>Select <strong>+</strong>-><strong>Net</strong>-><strong>HTTP Post</strong>.</li>
<li>Configure the <strong>Server:Port</strong> field and <strong>Path</strong> as needed and enter the %LOC_LOCATION and %LOC as appropriate values to whatever keys your service needs. Then select <strong>Done</strong>.</li>
</ul></li>
</ul></li>
</ul>




---

All content is licensed under [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/).
