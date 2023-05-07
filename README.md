Download Link: https://assignmentchef.com/product/solved-ence361-week-1-the-oscilloscopes-and-function-generators
<br>
<h1>  Learning outcomes</h1>

<ul>

 <li>Students become familiar with the use of the oscilloscopes and function generators on the benches in the Electronics Lab.</li>

 <li>Students learn how to generate and check the amplitude of a sinusoid and of a digital pulsed signal in the range 0 to 3 V.</li>

 <li>Students learn how to generate and check a variable DC voltage, also in the range 0 to 3 V, from the bench power supply using the oscilloscope and a digital multimeter (DMM).</li>

 <li>Students learn how to use the oscilloscope to measure the amplitude range and frequency of periodic signals, plus the pulse width and duty cycle of digital pulsed signals.</li>

</ul>




<h1>3.                 Laboratory Books</h1>




A physical lab book is <strong>strongly</strong> encouraged for all lab and project work in ENCE361, beginning with the formal lab sessions in Week-2. You should bring and use your lab book to every lab session to <em>neatly </em>jot down test data and take notes (sketches are also encouraged). Waveforms can also be captured and printed; these can be stuck into your lab book either with glue or clear tape. Include a date and subject title for every session.




See <em>“Keeping a Good Laboratory Records Book” </em>on the “Projects and Laboratories” page of the ENCE361 Learn site.




<h1>4.                 Lab procedure</h1>

Complete as much of this laboratory as you can within your allocated 2-hour lab session. Depending on your experience you may be finished within a shorter period.  Don’t be despondent if you do not complete everything.  You may also access the Electronics Lab at other times during normal working hours, Mon – Fri, provided it is not being used for other formal lab sessions.

<strong> </strong>    5.          The Agilent DSO-X-2012A Oscilloscope (see Figure 1)

The Agilent DSO-X 2012A oscilloscope on your desk can measure a range of parameters, such as the amplitude of a voltage signal, peak-to-peak voltage, frequency and duty cycle, to name only a few.  It can display and measure two independent signals simultaneously.




<strong>Figure 1</strong>: Agilent DSO-X-2012A Oscilloscope

To demonstrate these features, connect the 50Ω output from the signal generator directly to Channel 1 of the oscilloscope using a ‘BNC-to-BNC’ cable, as shown in Figure 2.

BNC connectors are pushed in and twisted slightly clockwise to lock.

Set the function generator to output a 1 kHz, 1 V peak-to-peak sine wave. Press ‘Autoscale’ on the oscilloscope to quickly display the waveform.  The ‘1’ button above the oscilloscope input should be glowing green, indicating that Channel 1 is active. In contrast, the ‘2’ button above the adjacent input should not be illuminated. Push each button a couple of times to individually activate and deactivate the different channels.

<strong>Figure 2</strong>:  The output of the function generator connected to the oscilloscope with a  BNC-to-BNC cable.

You can control the voltage (vertical) and time (horizontal) scaling on the oscilloscope display by turning the relevant knobs, as shown in Figure 1.

You can also measure various properties of the waveform using the ‘Measurement Type’ menu. Firstly, press the ‘Meas’ button on the oscilloscope and make sure that Source 1 is selected by pressing the far-left soft key.   If the label above it does not say ‘Source 1’, press the soft key repeatedly to change between available sources.   Next, select the property to be measured by pushing the second soft key from the left.  This brings up a list of options (shown in Figure 3), which can be cycled through either by pressing the soft key again or by turning the parameter knob.




<strong>Figure 3</strong>:  Soft keys on the oscilloscope screen.

<h1>6.          The Function Generator (FG) (See Figure 4)</h1>

The Electronics Lab benches are equipped with the TTi TG550 function generator.

<strong>Figure 4</strong>:  The TTi TG550 function generator.

Power on (the power switch is on the <strong>back</strong> of the unit).

Connect a <strong>BNC to alligator clips cable</strong> (see Figure 5) to the output (Push and twist the BNC cable to connect to the MAIN OUT connector fo the function generator) making sure the two alligator clips at the other end of the cable are not touching.

<em>These cables are always in short supply.  Do not steal one from another bench; ask Randy Hampton or a TA if you cannot locate one on your bench.  </em>

Connect a <strong>scope probe</strong> (see Figure 6) from the oscilloscope to the red alligator clip and connect the black clips from each cable together.  Of course, connecting like this should be identical to using the direct BNC-to-BNC cable; the difference is that the signal and ground connections are available for connecting to external systems.







<strong>Figure 5</strong>:   BNC-to-alligator-clips cable             <strong>Figure 6</strong>: Oscilloscope probe.  (<strong>signal – red</strong>; <strong>ground – black</strong>)




Next, select a sinusoidal waveform on the function generator and adjust the frequency control (see

Figure 4) to 1200 Hz and the amplitude control to 2.5 V<sub>p-p</sub>. Note that you will need to adjust the <strong>DC OFFSET</strong> control to obtain an offset of +1.25 V, so that the waveform should vary over the range 0 to 2.5 V.




Push <strong>Autoscale</strong> on the scope. The display should look similar to the trace in Figure 3.  What is different between what you see on the oscilloscope screen and what you expected?  Check the amplitude shown.

<strong><em>VERY important point:</em></strong>  The function generators in the Electronics lab are designed to output into a <strong>50 </strong>W<strong> load</strong> (i.e., the equivalent of a 50W resistor between the active output and ground). The oscilloscope <strong>and the input pins on the Tiva board</strong> have a much higher input impedance and therefore the actual voltage generated is <strong>higher</strong> than displayed on the display of the function generator.

<strong>EVERY TIME you connect a function generator to your Tiva board, check using the oscilloscope that you have a voltage range that does not go outside 0 to 3 V. </strong>

Next, adjust the function generator to give a square wave signal 0 to 3 V (as measured by the scope).  The amplitude setting displayed on the function generator will be less than half the actual voltage value.  Note the function generator <strong>Amplitude</strong> and <strong>Offset</strong> values (right on the LCD) for future reference (although they may vary between units).




Lastly, generate a full range (0 to 3 V) sinewave and a full range (0 to 3 V) triangular wave.  <strong>In each case, measure the RMS voltage (see the RMS handout in the lab folder) and compare this with what you calculate for the 3 V<sub>p-p</sub> waveforms. </strong>




<em>NB: if the waveform is offset, it does not have a mean value of zero. </em>




<h1>7.     Bench Power Supply and Digital Multi Meter (DMM)</h1>




Disconnect the function generator.

Connect one of the “<strong>30 V 2A</strong>” terminal pairs of the bench power supply to the Digital Multimeter (DMM) on the bench.  Use two banana-to-banana leads (preferably one red, one black, but this colour is not essential). Use the <strong>V</strong> input to the DMM for the red lead and the <strong>COM</strong> input for the black lead.  Set the DMM selector to <strong>V</strong><strong>—</strong> (DC voltage).

Note that the power supply has two “<strong>30 V 2A</strong>” outputs (variable voltage and current limit) plus one fixed DC output with two settings.  Each of the terminal pairs on the supply acts like a battery:  it has a positive and a negative terminal.  For example, to provide a constant +3 V to a Tiva GPIO pin, the negative terminal is connected to ground (rightmost terminal) on the supply front panel and to a Tiva ground pin; the positive terminal is then connected to the Tiva input pin.




<strong><em>Always check the connections carefully before turning the power supply output on. </em></strong>




Adjust the power supply voltage to 3 V according to the front panel display.  Turn the output ON and confirm the voltage with the meter.




The <strong>Current</strong> setting is to limit how much current the power supply can supply; 0.1 A should be adequate for your work in this course.  This limit is displayed when the output is OFF; the actual current is displayed when the output is ON.




<em>The current display is in amps (A) so probably will not show any more than</em> <strong>0.00 </strong><em>with the output ON. </em>

<em> </em>

When normally using the DMM you will need banana-alligator cables, as shown in Figure 7.










<strong>Figure 7</strong>: Banana-to-alligator-clip cables







<h1>8.     Final check and tidy up</h1>




Make sure that all bench equipment is turned off (unless someone else is waiting to use it). Please logout of the PC if you have used it, tidy up your bench, and place all spare leads neatly in the drawers where you found them. You need to follow this procedure after every lab session.





