## best way to program sending out custom text message in nokia

- posted by: [iamserious](https://stackexchange.com/users/-1/803-iamserious) on 2010-08-09
- tagged: `sms`
- score: 0

<p>Hi there,</p>

<p>I have a Nokia N97 Mini,
and I am planning to write a small utility which sends out text messages (sms) to selected people at selected file, all from a csv file which i will be modifying from my laptop..</p>

<p>anyway, my main concern is to write a code which sends out text messages. I looked at developer forums and the options were Nokia QT, J2ME, and then there was some C++ oriented language. </p>

<p>But the trouble was that I could not find any tutorials on how to program.. not even the basic stuff!</p>

<p>Can anyone please tell me what is the best way to code for this, and are there any tutorial sites on this?</p>

<p>Many thanks!</p>

<p>I'm not much of a java guy, I just know the basics.. but I am more into c# and c++</p>



## Answer 1220

- posted by: [John](https://stackexchange.com/users/-1/77-john) on 2010-08-09
- score: 0

<p><a href="http://stackoverflow.com/">http://stackoverflow.com/</a> is the best place to ask programming questions however to answer your question....</p>

<p>It really depends on if this is a one off app or you want to sell/distribute it.</p>

<p><strong>Nokia QT</strong><br>
I have never heard of Nokia QT however a quick look like phone gap and other systems that have their own easy to lean language which then converts it to a range of other languages/platforms. These are usually good as they are quick to learn and easy to use however they are are often limited to features they are willing to support and community help may be limited to people if there is a small fan base.</p>

<p><strong>J2ME</strong><br>
Java and C# are very similar and switching between the two should be easy. Writing in Java via J2ME will be quicker and will allow your app to run on more than one make of phone. Java also manages memory which will help reduce errors in your code. I think this is the best option if you are looking to distribute a stable app as there is a large community willing to help.</p>

<p><strong>C++</strong><br>
Anyone that has used C++ will know it will take longer to develop than other methods but you will have the maximum amount of control The application is also likely to run faster.</p>

<p><strong>Other Option</strong><br>
The other option is just to write the app for use on your laptop and use your phone as a GSM modem to send the SMS messages or use a web based SMS sending service.</p>

<p>Hope this helps</p>




---

All content is licensed under [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/).
