Library implementing sleep modes, allowing extremely low power consumption on Arduino based projects.

Narcoleptic uses the sleep functionality of the AVR microcontroller to almost completely shut down the entire CPU, just leaving a low power timer running to trigger the wake up.


Extract the download, and install in your Arduino Libraries directory. Restart Arduino and you will see the Narcoleptic library appear in the menus.

Syntax:

Narcoleptic.delay( time in milliseconds )


Note that Narcoleptic timings are only accurate to a few percent. Whilst sleeping, everything is stopped - including PWM outputs, the millis() timer, serial ports - everything. So code with this in mind.