## Does any eReader support CHM?

- posted by: [Ian Boyd](https://stackexchange.com/users/-1/1030-ian-boyd) on 2010-08-29
- tagged: `ebook`, `e-reader`, `ebook-reader`, `e-ink`
- score: 1

<p>Does any eReader support CHM?</p>

<p>i currently read CHM files on iPhone using a CHM app, but it's just too small actually read; so i'm looking to get an eInk based eReader.</p>

<p>But it has to support CHM - as i'm not converting them to other formats.</p>

<p><strong>Edit:</strong> The problem with converting to a PDF is managing to get</p>

<ul>
<li>being able to increase text-size, and reflowing the content</li>
<li>links maintained</li>
<li>no cut-off text, or text that runs off the end of the virtual A5 page.</li>
</ul>



## Answer 1637

- posted by: [Broam](https://stackexchange.com/users/-1/185-broam) on 2010-08-30
- score: 1

<p>CHM is one of those proprietary Microsoft formats I doubt many e-Readers are rushing to support. Your best bet is probably one of the Android-based ones that allows side-loading, and hoping that some enterprising hacker manages to put an application together to read CHM.</p>



## Answer 1653

- posted by: [Edwin](https://stackexchange.com/users/-1/1038-edwin) on 2010-08-31
- score: 1

<p>I have an eReader from Onyx, the Boox 60, which supports .CHM directly.  </p>

<p>Haven't used the feature before, but a short test viewing xunit-1.6.1.chm showed:  </p>

<ul>
<li>links are maintained  </li>
<li>increasing text size does reflow text.  </li>
<li>Text cuteoff depending on which page is viewed: for example:<br>
 "Namespaces > XUnit > Assert" no cutoff and reflow<br>
 "Namespaces > XUnit " Cutoff on rightside (as it also does in the desktop windows help viewer)  </li>
</ul>

<p>So how well CHM is displayed on the eReader depends also on the original page formatting.  </p>



## Answer 1643

- posted by: [MatthewMartin](https://stackexchange.com/users/-1/359-matthewmartin) on 2010-08-30
- score: 0

<p>You might be better off converting the chm to html before attempting to read it.</p>

<p>For example: <a href="http://www.gridinsoft.com/chm.php" rel="nofollow">http://www.gridinsoft.com/chm.php</a></p>

<p>or <a href="http://www.ubuntugeek.com/how-to-convert-chm-files-to-html-or-pdf-files.html" rel="nofollow">http://www.ubuntugeek.com/how-to-convert-chm-files-to-html-or-pdf-files.html</a></p>

<p>Ideally you'd want to get the chm to convert to a single great big XHTML file so that it would be easy to convert to mobi or kindle format</p>



## Answer 1645

- posted by: [Lorenzo](https://stackexchange.com/users/-1/155-lorenzo) on 2010-08-31
- score: 0

<p>I'm not aware of any eBook reader that directly supports CHM, you have to convert them to a supported format with a tool like MobiPocket.</p>



## Answer 1652

- posted by: [Davy Landman](https://stackexchange.com/users/-1/302-davy-landman) on 2010-08-31
- score: 0

<p>Because CHM is just a archive around a bunch of HTML, CSS and image files you could manually extract it (using 7zip) and run the html through a smart conversion tool.</p>

<p>Or use Calibre, which has given me some nice CHM -> ebook conversions.</p>




---

All content is licensed under [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/).
