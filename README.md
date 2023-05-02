# certbotzimbra
Script to automatise the deploy of certbot ssl on Zimbra mail server


Zimbra need the root CA inside the chain. This script automatise this procedure.


Note: is necessary to have the hostname correctly configured.
You can read more about in the header of the script


Put this script in 

 /usr/local/sbin/letsencrypt-zimbra


Make it executable

 chmod +x /usr/local/sbin/letsencrypt-zimbra


Set cronjob to automatise renew:

 ln -s /usr/local/sbin/letsencrypt-zimbra /etc/cron.daily/letsencrypt-zimbra


Edit /etc/crontab to set the hour of execution


Editor: Luca Piccinini <support@lpsystem.eu>
