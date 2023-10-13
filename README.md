This repository contains vi's required for using a two-microphone impedance tube. 

Download ASTM E1050 and read it carefully.

It is assumed that you have moderate knowledge of using LabView because you have to adjust some parameters based on your design.

Download all the files and run main.vi.

Buy a pair of electret microphones, a speaker, an amplifier and a dual channel sound card and circuit them up based on ASTM E1050. Refer to the solid works design drawing.

Refer to the AliExpress file for retailers of the electric components (Provided in the Electronics folder).

Find the drawings of the impedance tube in the Drawings folder.

You must connect a portable sound card with dual channel input and output sockets.

It is recommended to disable all the sound input and output hardware in your operation system except those you use as input (Lin-in) and output for your impedance tube.

In main.vi, hit store params to create config.ini. Based on your design, you need to adjust the default values of the variables "l" and "s", which are the distance from the sample surface to the first microphone and microphone spacing. Choose them with an accuracy of 1 mm. You need to calculate air density and speed of sound based on air environmental conditions. Use air temperature and your altitude to calculate these values. In main.vi, in the Test Parameters tab, choose the correct device number of speaker and microphone devices; if you have disabled other devices, they should be zero. Maximise your speaker volume in Windows before doing a test. Also, adjust the default value of the upper frequency based on your impedance tube design. 

You need to run Calibration first. It generates Hc (Refer to ASTM E1050). You have to swap the microphones twice. The results get stored in Correction. ini

Then, you can Run A Test

Happy building your own impedance tube and customising the software based on your design!

Any questions: mabiran@gmail.com
