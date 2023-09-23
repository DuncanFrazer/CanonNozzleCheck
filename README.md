# CanonNozzleCheck
Canon MG5750 nozzle check file with automation to send once a week and exercise the heads &amp; ink tanks

setup a cron job on a raspberry pi with
crontab -e

add this cron command to print the nozzle check every sunday evening at 7pm local time
0 19 * * 0 lp -d Canon_MG5700_series ~/Documents/MG5750_nozzle_check.SPL

change the cron scheduling numbers to change the schedule
https://crontab.guru/#0_19_*_*
