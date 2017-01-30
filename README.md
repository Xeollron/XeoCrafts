Xeocraft# Scipts

Script for running and managing minecraft (normally forge modded) servers.
Uses ramdisk for storage and has inegrated backup and archival features.


Configuration located at start of script

SERVICE= minecraft or forge server jar

MCSTORE= directory of minecraft server on disk

MCPATH= server ramdisk mount point and running directory

BACKUPPATH= directory for backups to be stored

OFFBACKUPPATH= secondary, long term backup directory

CRASHLOG_DB_PATH= directory to dump server crash logs

JAVA_HOME= directory where java is installed

MEMORY_OPTS= minecraft server memory allocation in format "-Xmx#G -Xms#G" replace # with amount of allocated RAM in GB

DISKSIZE= size of ramdisk allocation, must be larger than server files

JAVA_OPTIONS= extra options for the JVM to try to optimize for minecraft


dependancies/requirements:
	BASH > version 4.X,
	tmux,
	java jre (preferably 8 oracle)

Usage: xeocraft [server number] {start|stop|restart|backup|exec|dumpcrashlogs|disksavehalt|disksaverun|status|open}
