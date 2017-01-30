Xeocraft# Scipts

Scripts for running and managing minecraft (normally forge modded) servers.
Uses ramdisk for storage and has inegrated backup and archival features.
lite version designed for VPS use, excludes ramdisk and archival.


Configuration located at start of script

SERVICE= minecraft or forge server jar

MCSTORE= directory of minecraft server on disk (not on lite)

MCPATH= server ramdisk mount point and running directory

BACKUPPATH= directory for backups to be stored

OFFBACKUPPATH= secondary, long term backup directory (not on lite)

CRASHLOG_DB_PATH= directory to dump server crash logs

JAVA_HOME= directory where java is installed

WRPATH= driectory where warmroast jar is located (only needed for debug functions, only on lite currently)

MEMORY_OPTS= minecraft server memory allocation in format "-Xmx#G -Xms#G" replace # with amount of allocated RAM in GB

DISKSIZE= size of ramdisk allocation, must be larger than server files (not on lite)

JAVA_OPTIONS= extra options for the JVM to try to optimize for minecraft


dependancies/requirements:

	BASH > version 4.X
	
	tmux
	
	java jre (preferably 8 oracle [server])
	
	warmroast (for debug funtions, only on lite currently)
	

Usage: xeocraft [server number] {start|stop|restart|backup|exec|dumpcrashlogs|disksavehalt|disksaverun|status|open|debugon|debugoff} 
