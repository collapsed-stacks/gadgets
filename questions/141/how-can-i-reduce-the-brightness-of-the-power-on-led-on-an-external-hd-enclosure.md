## How can I reduce the brightness of the power on LED on an external HD enclosure?

- posted by: [Dennis Williamson](https://stackexchange.com/users/-1/89-dennis-williamson) on 2010-07-14
- tagged: `harddrive`, `led`, `brightness`, `enclosure`, `tinker`
- score: 2

<p>I have an external hard drive enclosure with a blue LED to indicate power on. I believe it's a dual color LED because I can just <strong><em>barely</em></strong> see a red flash when there's activity on the drive. I re-opened the enclosure (after having installed the drive and seeing the brightness) and if I remember correctly there is a three-conductor cable going to the LED so I think they are driven separately instead of by polarity reversal.</p>

<p>The blue LED is so bright I don't need other room illumination (this is only a <em>slight</em> exaggeration).</p>

<p>Short of covering the light with duct tape (perhaps with a pinhole), how can I control the brightness of the blue LED? Ideally, the red LED would be usefully visible as a result.</p>

<p>I posted this here since it seems to be more about an electronic gadget than a computer peripheral.</p>



## Answer 146

- posted by: [ajray](https://stackexchange.com/users/-1/40-ajray) on 2010-07-14
- score: 2

<p>Without going into too much detail, if you reduce the current through that side of the diode (green side instead of red side) it'll get dimmer.  I have no idea what the circuit looks like inside, but in most cases <strong>it's possible to put a small (low-value) resistor in series with the green side of the LED and make it dimmer</strong>. this will take some experimentation, and you might want to try using a potentiometer (variable resistor) to figure out what value of resistor you need.</p>

<p>Other than that it might be pretty straightforward to cut it out and use an external green LED (they're super cheap) soldered in its place in the circuit that's displaced 1-2" from the red LED so its clear when each is on or off (you could do this to the red one as well.  Essentially, <strong>cutting one side of the two-color LED off and replacing it with another LED 1-2" away.</strong></p>

<p>Notes:</p>

<p>requires some rudimentary knowledge of circuits and soldering.</p>



## Answer 166

- posted by: [Niall C.](https://stackexchange.com/users/-1/87-niall-c) on 2010-07-14
- score: 2

<p>Low tech solution: could you cover it with something translucent and red to filter out most of the blue?</p>

<p>(I've been trying to think of readily available translucent red materials.  I think some older-style 3-D glasses have a red lens; maybe multiple layers to get the blue level down low enough.)</p>




---

All content is licensed under [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/).
