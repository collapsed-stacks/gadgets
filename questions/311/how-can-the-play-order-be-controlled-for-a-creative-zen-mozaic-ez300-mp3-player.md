## How can the play order be controlled for a Creative ZEN Mozaic EZ300 MP3 player?

- posted by: [Peter Mortensen](https://stackexchange.com/users/-1/118-peter-mortensen) on 2010-07-15
- tagged: `mp3-player`, `creative`, `play-order`, `zen-mozaic-ez300`
- score: 1

<p>How can I externally control MP3 file play order for a Creative <a href="http://en.wikipedia.org/wiki/Creative_ZEN#ZEN_Mozaic" rel="nofollow">ZEN Mozaic EZ300</a> MP3 player?</p>

<p>By externally I mean one or more of:</p>

<ul>
<li><p>setting file and/or folder time stamps (say, modification date or creation date) such that the time stamp order is the required play order </p></li>
<li><p>renaming files/folders such that the alphabetical order is the required play order </p></li>
<li><p>constructing special files that define the play order. </p></li>
</ul>

<p>Is this possible?</p>

<p>I have extensively tried the renaming and time stamping strategy, but with no success. Perhaps I have overlooked something.</p>

<p>I have had the same problem with earlier generations of MP3 players from Creative. But at least on the Creative Zen Stone there was a small button to jump to the next folder (it made this problem bearable). EZ300 does not even have this option (as far as I can tell).</p>



## Answer 1322

- posted by: [Peter Mortensen](https://stackexchange.com/users/-1/118-peter-mortensen) on 2010-08-13
- score: 1

<p>Yes, it is possible using a special file that defines the play order.</p>

<p>It turned out to be deceptively simple.</p>

<p>It can be done with <a href="http://en.wikipedia.org/wiki/Playlist" rel="nofollow">playlists</a>. Creative ZEN Mozaic EZ300 supports <a href="http://en.wikipedia.org/wiki/M3U" rel="nofollow">M3U</a> playlist files (file extension .m3u). If an M3U file with the right content is copied to folder "Playlist" on the ZEN Mosaic then the MP3 files can be played in the desired order.</p>

<p>A complication is that ZEN Mozaic EZ300 requires <a href="http://en.wikipedia.org/wiki/8.3_filename" rel="nofollow">8.3</a> DOS file names in the M3U file. E.g. the file <code>HerdingCode-0090-Sara-Chipps-on-GirlDevelopIt-and-Girls-Developing-Software.mp3</code> must be listed as e.g. <code>HERDIN~1.MP3</code>.</p>

<p>Software exists to automate this process, but I describe the manual process below. It also a way to demonstrate what such software does.</p>

<hr>

<p>Example:</p>

<p><strong>1. The files</strong></p>

<p>ZEN Mozaic EZ300 is connected through USB to a Windows computer, drive G:. There are 6 files in folder <code>G:\Podcasts\temp102</code>:</p>

<pre><code>    dotnetrocks_0583_jay_schmelzer.mp3
    grammar058-however_StartingA_SentenceWithHowever.mp3
    harddisken_2010-08-11.mp3
    HerdingCode-0090-Sara-Chipps-on-GirlDevelopIt-and-Girls-Developing-Software.mp3
    sn0261.mp3
    twig0055.mp3
</code></pre>

<p><strong>2. The filename transformation</strong></p>

<p>Find 8.3 names for long file names using a Windows command-line window (<kbd>Win</kbd> + <kbd>R</kbd> + <kbd>cmd</kbd> + <kbd>Enter</kbd>):</p>

<pre><code>    G:
    cd G:\Podcasts\temp102
    dir /X
</code></pre>

<p>Output is (edited for clarity):</p>

<pre><code>    DOTNET~1.MP3 dotnetrocks_0583_jay_schmelzer.mp3
    GRAMMA~1.MP3 grammar058-however_StartingA_SentenceWithHowever.mp3
    HARDDI~1.MP3 harddisken_2010-08-11.mp3
    HERDIN~1.MP3 HerdingCode-0090-Sara-Chipps-on-GirlDevelopIt-and-Girls-Developing-Software.mp3
                 sn0261.mp3
                 twig0055.mp3
</code></pre>

<p>The alternative to finding 8.3 names is to rename the files.</p>

<p><strong>3. Create the playlist file</strong></p>

<p>Create an empty text file in <code>G:\Playlist</code> and rename it to <code>TechPodcasts1431.m3u</code>. Open it in Notepad (or your favourite text editor) and add:</p>

<pre><code>\PODCASTS\TEMP102\DOTNET~1.MP3
\PODCASTS\TEMP102\GRAMMA~1.MP3
\PODCASTS\TEMP102\HARDDI~1.MP3
\PODCASTS\TEMP102\HERDIN~1.MP3
\PODCASTS\TEMP102\sn0261.mp3  
\PODCASTS\TEMP102\twig0055.mp3
</code></pre>

<p>There should be a empty line after the last file (<code>twig0055.mp3</code>). I emperically established that the file will not turn up in the playlist if it is left out.</p>

<p>This playlist file will result in a playlist named "TechPodcasts1431".</p>

<p><strong>4. Play</strong></p>

<p>Unmount the ZEN Mosaic and turn it on.</p>

<p>Do:</p>

<blockquote>
  <p>menu Music/Playlists/&lt;select TechPodcasts1431>/open/select the first/open/Play</p>
</blockquote>



## Answer 1482

- posted by: [mihi](https://stackexchange.com/users/-1/956-mihi) on 2010-08-20
- score: 0

<p>With most "simple" players that use the FAT filesystem, they just play in the order the files are in the root directory list. As changing a file will not change the place of the file in there (assuming the name does not get longer in case of vfat), and deleting a file will make a new space where the next file might be stored, the easiest way usually is to create a completely new folder on the device (best with mkdir on the command line) and then use a batch file to move every file into that folder (one file per move command). The files will be played in that order afterwards. To re-order, rename the folder, create a new with the old name again and move the files back.</p>

<p>Can be automated quite well (just leave the batch script on the device).</p>




---

All content is licensed under [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/).
