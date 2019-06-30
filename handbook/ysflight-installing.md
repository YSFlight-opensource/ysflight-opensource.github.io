# YS FLIGHT SIMULATOR (フリー) HANDBOOK

Handbook rev.2019/04/25 for YSFlight ver.20181124 and older.

```
Copyright 2019 (CC-BY-SA 4.0) u2fly, forum.YSFHQ.com & contributors
```

[Table of Contents](index.md) | [← Introduction](introduction.md) | [YSFlight Configuration Files →](ysflight-configuration-files.md)

***

## YSFLIGHT INSTALLING

YS FLIGHT SIMULATOR (YSFlight) — is FREE flight simulator game for PC.

- DOWNLOAD — [http://ysflight.com](http://ysflight.com) ([mirror](http://ysflight.in.coocan.jp)) or [ysflight.org/download](http://ysflight.org/download)

- PLATFORM / OS:	Linux (32bit & 64bit), Mac OS X (64bit), Windows (32bit & 64bit)

After downloading correct binary package install it as other programs on your OS.

It's already distributed for different graphic cards & drivers: DirectX, OpenGL1.x, OpenGL2.

> OpenGL2 version produce best  graphic quality, but need more powerfull GPU for run.

### LAUNCH SETUP & RUN

You can start YSFlight executable in few ways:

- by clicking on executable file;

- run from console with parametres (see bellow).

On Linux there is support for ALSA and Pulse-Audio backend:

- ALSA plug-in (used by default):
  - `../plugin/sndYsflight32.so`
  - `../plugin/sndYsflight64.so`
- Pulse-Audio plug-in:
  - `../plugin/sndYsflight32-pulse.so`
  - `../plugin/sndYsflight64-pulse.so`

If ALSA not work for you try use Pulse-Audio by default. For this rename delete files of ALSA plug-in and rename `sndYsflight**-pulse.so` to `sndYsflight**.so` and restart YSFlight.

### RUN FROM CONSOLE

Using “YSFLIGHT Command Parameters” you can run in needed mode directly from console.

```
-h 
  -help 
   Show help. 

  -keymenu 
   Use key menu. 

  -configdir Path 
   Override user-configuration directory.

  -userdir Path 
   Override user YSFLIGHT directory.

  -replayrecord Filename 
   Replay flight record. 

  -freeflight Airplane Field Position 
   Fly Free Flight. 

  -flyyfs Filename 
   Load .YFS and fly. 

  -endurance Airplane Field NWingmen WingmenLvl UseMissile 
   Endurance Mode (15 minutes dogfight) 
     NWingmen    : 0 to 2 
     WingmenLvl  : 1 to 5 
     UseMissile  : 0(not use) or 1(use) 

  -intercept Airplane Field Stealth Escort HeavyBomber Bomb NEnemy NWingmen 
   Intercept Mission (15 minutes base defense) 
     Stealth     : 0(not allow stealth) or 1(allow stealth) 
     Escort      : 0(not allow fighter escort) or 1(allow fighter escort) 
     Bomb        : 0(not allow bomb) or 1(allow bomb) 
     NEnemy      : 1 to 5 
     NWingmen    : 0 to 2 

  -server Username 
   Start server mode. 

  -client Username ServerHostName 
   Start client mode. 

  -netport portNumber 
   Specify port number. 

  -autoexit 
   Exit after flight. (Ignores -keymenu.) 

  -saveflight Filename 
   Save after flight. 

  -listairplane 
   Show airplane list. 

  -listfield 
   Show field list. 

  -liststartpos Fieldname 
   Show start position list. 

  -setdefaultconfig 
   Set default configuration. 

  -setdefaultnetconfig 
   Set default network configuration. 

  -setdefaultkeyassign 
   Set default keyboard assignment. 

  -setdefaultoption 
   Set default option. 

  -english 
   Force English mode. 

  -language [languageString] 
   Force to use given language string (eg. en for English, ja for Japanese.)
```

Additionally here is eastern-egg command, not shown from `-help` in console:

```
  -demoforever 
   Run YSFlight in demonstrating mode!
```

By default, in `-demoforever` mode used only two stock sceneries, but you can change it to own by editing `../scenery/scenery.lst` file (for details read chapter .LST file)

> Sometime OpenGL output FPS is low, then you can try increase it (tested on Linux).
>
> If you have Intell, ATI/AMD or other GPU then try next command:
>
> ```
> ~ $ vblank_mode=0 {path-to-ysflight-executable}
> ```
>
> If you have GPU provided by NVIDIA with “OPTIMUS” technology and PC under Windows (or read about “Primus” and “Bumlebee” technology for Linux) try use one from next commands:
>
> ```
> ~ $ vblank_mode=0 primusrun {path-to-ysflight-executable}
> ```
>
> or
>
> ```
> ~ $ optirun {path-to-ysflight-executable}
> ```
>
> Also read more about “PRIME” technology for Intell, ATI/AMD or other GPU in its docs.

***

[Table of Contents](index.md) | [← Introduction](introduction.md) | [YSFlight Configuration Files →](ysflight-configuration-files.md)
