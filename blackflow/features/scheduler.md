# ⏰ Scheduler

Campaign scheduler is a bot that will auto start and auto pause campaign on the time and day you chose.

It's useful because most of the offers have ON hours where you get most of the traffic and higher CR. Letting campaign live at night increase the risk of getting your campaign banned. Scheduling your campaign reduce risk of getting banned by 50%

![Screen Shot 2020-03-18 at 11.12.20 AM.png](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/03/20-15-49-12-Screen%20Shot%202020-03-18%20at%2011.12.20%20AM.png)

#### How it works ?

The timezone is UTC so you need to adjust based on that.

* Ie you launch a campaign in USA from 8h to 20h local time GTM-4 , you need to convert schedule to 12:00 - 24:00
* Ie campaign in Germany from 8h to 20h local time GTM+1 , then schedule is 7:00 - 19:00

What else to know:

* The scheduler run every 30min, so if you set 9:15 as it will count as 9:30 anyway
* Make sure to tick the box schedule to make the bot active.

