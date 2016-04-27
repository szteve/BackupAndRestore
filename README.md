#BackupAndRestore
#Software Installation Assignment 

This code allows the user to backup and restore specified
files on a linux system to the root of the system
where it will be safe, the cronback file also allows the user to
schedule backups for the system to run monthly week etc

#Instructions

1.Download this repo to your system using this command in your terminal
  git clone https://github.com/szteve/BackupAndRestore

2.cd into the repo using: cd BackupAndRestore

3.Compile the two codes individually using 

  sudo chmod 775 backup NOTE: must have password for sudo to work

			      if you dont know password you shouldnt

			      be backing up the SYSTEM!!

4.use following command to run the script

  sudo ./backup

5.Follow the instructions on the menu

#Instructions to schedule backup

1.Download cron using this command

  sudo apt-get install gnome-schedule

2.Enter command: sudo crontab -e to schedule a backup

3.In new screen thats opened hit i and type without

  hash symbol: 01 04 * * * /usr/bin/somedirectory/somecommand

  NOTES:      Min Hr Day Month Weekday /desired path of command

	      which in this case is CronBack 

4.Then the backup command should backup designated files on

  the schedule desired
