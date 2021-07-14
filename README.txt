**** cherryJB ver 1.6.0 [1F79] ****

made by twitter-ID: @dora2ios

*whats?
-+ untethered jailbreak or downgrade tool using iboot7 exploit

*** important note ***
- This tool exploiting iOS 7 iBoot. Therefore, you need an iOS 7 SHSH blob.
- For iPhone 4, iOS 7.1.2 be signed by Apple. Select iOS 7.1.2 IPSW after the -derebusantiquis flag.
- Otherwise, choose the iOS 7 IPSW that matches the SHSH blob you have.
- Currently only available on iPhone 4 and iPhone 5 with iOS 7.1.x SHSH. If you want to check the progress, please see "TODO.png".

*How to confirm which version or devices are supported?
	./cherryJB --version <device>

*How to use
-+ make CFW [Have JB]
	./cherryJB <in> <out> -j -memory -derebusantiquis <7.1.x ipsw>

-+ [NoJB]
	./cherryJB <in> <out> -memory -derebusantiquis <7.1.x ipsw>

*Restore iOS firmware
-+ iPhone3,1 [limera1n devices]
	./iPwnder32 -p
	./idevicerestore -t <7.1.2 ipsw>
	mv -v shsh/[ECID]-[device]-7.1.2.shsh shsh/[ECID]-[device]-[iOSver].shsh
	./idevicerestore -e -w <out>

-+ iPhone5,2 [armv7 checkm8 devices]
	./iPwnder32 -p -b
	mv -v 7.1.x.shsh shsh/[ECID]-[device]-[iOSver]-[BUILD].shsh
	./idevicererestore -r <cfw.ipsw>


(ex) untethered iOS 9.3.5 jailbreak with 7.1.2 SHSH (for iPhone5,2)

	 ./cherryJB iPhone5,2_9.3.5_13G36_Restore.ipsw Custom.ipsw -j -memory -derebusantiquis iPhone5,2_7.1.2_11D257_Restore.ipsw
	
	~Connect device in DFU mode~
	
	 ./iPwnder32 -p -b
	 mv -v 7.1.x.shsh shsh/1234567890-iPhone5,2-9.3.5-13G36.shsh
	 ./idevicererestore -r Custom.ipsw

	~DONE~

*thanks
geohot for limera1n exploit
axi0mX for ipwndfu
xerub for De Rebus Antiquis
iH8sn0w for iBoot32Patcher
tihmstar, nyan_satan, Ralph0045, Merculous, and a8q for Improvement of iBoot32Patcher
libimobiledevice for idevicerestore
planetbeing for xpwn
dayt0n by Odysseus
synackuk for n1ghtshade
