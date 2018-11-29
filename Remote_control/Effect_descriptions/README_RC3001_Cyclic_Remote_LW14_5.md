# "RC 3001, cyclic control, B"  
Filename: RC3001_Cyclic_Remote_LW14_5.fx  
**WARNING: THIS EFFECT REQUIRES LIGHTWORKS 14.5 OR BETTER**
   
![Preview]( https://raw.githubusercontent.com/FxSchrauber/Images_for_effects_repository/master/RC/RC_3001_cyclic_control_Nov2018.png)

### Effect descriptions:
This is a version of the master controller for the remote control user effects subsystem
adds the ability to cycle the values of the effects channels.
This effect outputs the remote control signal on channel 3001.

### Compatibility:
In particular, if there are problems with the effect, I ask for feedback.
The effect should theoretically work across platforms, but until 29.11.2018 only a test on Windows was possible.


### Details: 
- Note 1, Assistent effect for correct adjustment:  
In particular, if a different cyclic waveform is to be set,
then it is recommended to add the effect "Setting Display Unit" at the end of the routing.

- Note 2, Remote control input:
What is connected to the input of the effect has no effect on the effect itself. 
However, the input can be used to pass the remote control signal from another remote control, 
which is transmitting on another channel, to the output. 
At the output of the effect then the remote control signals of both effects will be available. 
That also works with more remote controls.
If you do not need this feature, you can leave this input open.

- Note 3, Keyframing:
A sliding change of the "Interval" will lead to unexpected interval times.
The same applies to "Start delay", for which, however, only a static value makes sense anyway.

- Note 4, Export: 
   If the "Setting Display Unit" was used for the effect setting, then deactivate it for the final export.
  - Note 4b, when using the export option "Marked section": 
    The export always starts at the beginning of the interval curve. 
    This may differ from the playback if the starting point of the "Marked section" has been positioned 
    to the right of the beginning of the effect in the timeline. (interval phase shift between playback and export). 
  - "Start Delay" slider: Avoid positioning the "Marked section" within the effect time. 
    If this is not possible, please leave "Start Delay" at 0.

- Note 5, Cycle frames with decimal places : 
The cycle progress will occasionally pause for 1 frames
at a position to remain synchronized with the set value.


### Update (newest first):
29 Nov 2018 by LW user schrauber: Changed subcategory from "Remote Control" to "Remote control".  
19 Nov 2018 by LW user schrauber: Changed effect name  

10 Nov 2018 by LW user schrauber:  
Simplification of the effect settings.  
Interval setting is now switchable between frames and seconds.  
Reduction of GPU load.  
The quality of the signal transmission should now be independent of the GPU/OS.  
                                 
3. May 2018 by LW user schrauber:  
Unnecessary sampler settings removed.  
Subcategory defined, effect description and other data relevant to the user repository added.  

18 Feb 2017 by LW user schrauber:  
Status level of the blue transmission channel updated (standardization with the other remote control effects)  

