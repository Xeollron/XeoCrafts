Xeocraft# Scipts

Scripts for running and managing minecraft (normally forge modded) servers.
Uses ramdisk for storage and has inegrated backup and archival features.
lite version designed for VPS use, excludes ramdisk and archival(also currently heavily outdated).


Configuration file should be in ~/.config/xeocraft.config

dependancies/requirements:

	BASH > version 4.X
	
	tmux
	
	java jre (preferably 8 oracle [server])
	
	warmroast (for debug funtions, only on lite currently)
	

Usage: xeocraft [server number] {start|stop|restart|backup|archive|thinarchive|exec|opsay|slowrestart|safestart|disksavehalt|disksaverun|status}
