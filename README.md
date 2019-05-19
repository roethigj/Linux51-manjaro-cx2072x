# Linux51-manjaro-cx2072x
patch cx2072 codec and driver and USM files from 
Takashi Iwai: https://git.kernel.org/pub/scm/linux/kernel/git/tiwai/sound.git/log/?h=topic/soc-cx2072x-5.1 
into Manjaro 5.1 kernel

Thanks to all tha guys bringing input to this discussion: https://bugzilla.kernel.org/show_bug.cgi?id=115531

Maybe UCM didn't apply automatically. In this case you need to do: "alsaucm -c chtcx2072x set _verb HiFi" and "pulseaudio -k"
You may put this in a startup script. 
