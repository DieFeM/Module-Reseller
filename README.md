# Module-Reseller

Edit the cron tab:

crontab -e

and copy this line at the end of the file and save it (WARNING:modify it with the correct path):

*/30 * * * * php /var/www/html/modules/reseller/cron-shop.php

Now this script searches for expired game homes every minute, and wil stop and remove them if they are expired.
If you would like to do this at midnight every day instead of every minute you should use

0 0 * * * php /var/www/html/modules/reseller/cron-shop.php

TIP: Searching in google, for example, "crontab run job once a month" you will find the correct code to search expired homes and remove them every month.
