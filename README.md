# CanonNozzleCheck
Canon MG5750 nozzle check file with automation to send once a week to prevent the inks and heads from drying up

setup a cron job on a raspberry pi with
> crontab -e

add this cron command to print the nozzle check every sunday evening at 7pm local time
> 0 19 * * 0 lp -d Canon_MG5700_series ~/Documents/MG5750_nozzle_check.SPL


or this to print the nozzle check every 1st of the month at 8pm local time
> 0 20 1 * * lp -d Canon_MG5700_series ~/Documents/MG5750_nozzle_check.SPL

change the cron scheduling numbers to change the schedule
https://crontab.guru/#0_19_*_*
