# Scheduling Tasks with Cronjobs in Linux

<h2>Description</h2>
In this Linux home lab, I scheduled a task to execute a ./backup.sh script from a previous lab using cronjobs.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Linux CLI</b> 

<h2>Environments Used </h2>

- <b>Linux Mint 22</b> 

<br />
<br />
The bash script to be used. 

![1) Bash script to be run](https://github.com/user-attachments/assets/431e68bd-457e-4f61-8825-9dc4537c894f)

<br />
<br />
Creating "hello world" text file in /Confidential. Confirming nothing is in /Backups.

![2) Confidential hello txt file to be copied into Backups](https://github.com/user-attachments/assets/81b30d73-3bb2-44a3-937e-6e3bddec86db)

<br />
<br />
Changed executable permissions for root user for backup.sh script. 

![3) gave root executable permission for backup sh](https://github.com/user-attachments/assets/b669f7ad-4bfd-4345-9881-95a9c0cc0c6b)

<br />
<br />
Wrote cronjob task for root to execute ./backup.sh script for 9:17am. 

![4) scheduled backup sh cronjob in crontab ](https://github.com/user-attachments/assets/55b63c27-2953-4336-82ae-6a79f7e0fff8)

<br />
<br />
Observe that cronjob executed the ./backup.sh script on 9:17am to copy files from /Confiential into a /$date directory in /Backups.

![5) Observe cronjob executed backup sh into Backups at 9:17 am](https://github.com/user-attachments/assets/d8a60d67-9bbf-4a90-8e89-142a30404695)

<br />
<br />
Confirm cronjob task was executed by checking the syslogs with sudo cat /var/log/syslog

![6) cconfirm cronjob execution with syslog check](https://github.com/user-attachments/assets/bca75fd2-fdf2-41b4-aa1f-bfdc6db33fad)

<br />
<br />
