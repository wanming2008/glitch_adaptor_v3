# glitch_adaptor_v3

Voltage glitching driver board using LM5134 and IRF7607.

This is designed for use with the ChipWhisperer-Lite. For best performance, physically remove or disconnect the built-in glitching FETs on the CW-Lite board and connect the gate drive signal to this glitching board via coax. The connection from glitch board to target Vcore signal should be very short, I used about a centimeter of twisted heavy-gauge magnet wire. The FET drivers run from 12.5 volts to get the fastest slew rates we can. This circuit switches in a capacitor bank to stabilize Vcore when not glitching, intended for use with chips that have a low voltage core with a built-in regulator.

Board layout for KiCad, thrown together for quick assembly using the parts I had on hand. You may want to substitute your favorite voltage regulators if you like.


