Some custom patches for building kitkat beanstalk.
=======

I don't know why but since kitkat release, I can't build fluidly anymore. About the build patch, I understand that the new zipping proccess is better but I don't want to change the custom of release script of galaxys4gmtd nor find it neccessary since we don't really have any problem with that.

But somehow the bionic project bug us as hell. It's like newer Android version is for high-end/newer phones, not for legacy ones even that Google stated once that Android support legacy phones well and not aimed to abandon them but I don't believe it. The bionic changes whacked off a file in the Makefile that is needed for our phone so I want to restore it. And we are sharing source with cortex-A15 anyway!

For the charger patch, it's not really a device failure but the recovery. As you all can see that I use TWRP instead of CWM and there's a change in charger.c aimed to support CWM updates but not TWRP yet so it is a temp for us as we all want TWRP, rite? Instead of CWM like Beanstalk officials.

The last thing is the build script that I adopted from Slimsaber. Thanks Fusionjack for it as I find it's kinda useful, especially in setting up the ccache.

These patch are, in some ways, universal for kitkat builds to be built properly atm for galaxys4gmtd. When I have time later, after my exams, I will clean up the build tree and make changes to adapt to AOSP best, instead of using temp patches so hopefully, this repo will be dis-continued soon. Cheers!
