## How can I send n-number automated messages to my phone every day?

- posted by: [Jeff](https://stackexchange.com/users/-1/356-jeff) on 2010-07-22
- tagged: `apps`, `home-automation`, `text-message`
- score: 3

<p>I need to use my phone (dumb, no internet capability) to 'ping' me a certain number of times per day. The alarm function will not work for this. This is a reminder to myself to do pushups throughout the day. Is there a way to generate, for example, 5 of the same text message and have it sent to my phone at 5 random times of day?</p>

<p>I also need to set a minimum time between messages, so two of them are not too close together. (i.e., I would have time to physically recover from the exercise).</p>



## Answer 610

- posted by: [Conrad Frix](https://stackexchange.com/users/-1/178-conrad-frix) on 2010-07-22
- score: 2

<p>You can use Windows Power Shell</p>

<p>The code below came from  <a href="http://www.searchmarked.com/windows/how-to-send-an-email-using-a-windows-powershell-script.php" rel="nofollow">here</a></p>

<pre><code>$emailFrom = "user@yourdomain.com"
$emailTo = "user@yourdomain.com"
$subject = "your subject"
$body = "your body"
$smtpServer = "your smtp server"
$smtp = new-object Net.Mail.SmtpClient($smtpServer)
$smtp.Send($emailFrom, $emailTo, $subject, $body)
</code></pre>

<p>This link describes what you need to do to enable the code for scheduling <a href="http://www.searchmarked.com/windows/how-to-schedule-a-windows-powershell-script.php" rel="nofollow">Here</a></p>

<p>Then you just use Windows scheduler. To schedule the script. </p>



## Answer 677

- posted by: [Greg Bray](https://stackexchange.com/users/-1/191-greg-bray) on 2010-07-24
- score: 1

<p>Google Calendar supports <a href="http://www.askdavetaylor.com/google_calendar_send_sms_event_notifications.html" rel="nofollow">SMS based notifications</a>. You can't set them to be random, but you could setup daily recurring events that send an SMS notification to you. If you want them to be at different times you could setup multiple weekly recurring events so that each day has a different schedule.  </p>



## Answer 605

- posted by: [txwikinger](https://stackexchange.com/users/-1/218-txwikinger) on 2010-07-22
- score: 0

<p>You can use an e-mail to SMS gateway, to send SMS text messages to your phone. Now, you just need a script that sends those e-mails to the gateway. </p>




---

All content is licensed under [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/).
