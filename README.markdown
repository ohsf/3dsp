#Modified 3DSP driver source

I tried to compile the 3DSP source available at [reyiyo repository](http://github.com/reyiyo/3dsp.git), but it didn't work with Ubuntu 12.04, so I made some changes in the code and it works for me.

First, you should install all dependencies:

    $ sudo apt-get install build-essential linux-headers-`uname -r` libnotify-dev libgtk2.0* blueman dhcpcd libgnome2-dev 
      git

With all dependencies satisfied, just clone this git repository: 

    $ git clone http://github.com/roqueboi/3dsp.git
    $ cd 3dsp
    
If you don't use git, just download the source from Github, extract it: and run Install\_3DSP.sh:

    $ curl http://github.com/roqueboi/3dsp/tarball/master -o 3dsp.tar.gz
    $ tar -xvzf 3dsp.tar.gz
    $ cd 3dsp

If you prefer to install applications 3dsp-wifi-radar and UWB translated into Brazilian Portuguese remove the applications directory and rename the directory applications_pt_br to applications:
    
    $ sudo rm -r applications
    $ sudo mv applications_pt_br applications

And run Install_3DSPUSB.sh:

    $ sudo bash Install_3DSPUSB.sh

If you are using Ubuntu with Unity desktop, the uWB and Wifi Radar icon will not appear in the systray. You will have to do one aditional step, that you can find it here:

(In spanish): http://tuamigotetieneganas.blogspot.com/2011/04/unity-area-de-notificacion-systray.html

I would give due credit to the great work of reyiyo and fsouza, who did fork the repository. Thank you for everything.

If you have any question, contact me: odilon.filho [at] gmail [dot] com

