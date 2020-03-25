Content

[quick start](#quick start), [scheduler,](#scheduler) [integration](#integration), [domain](#domain)

[lander](#lander), [offer](#offer)

# Quick start

WATCH THIS
https://www.loom.com/share/e1addf50bad84d14931278356e52126d

### What is this?

*Blackflow is the backend that bring all the piece of the puzzle together ( source, account, domain, safe page, money page, offer, cloaking, tracking )*

**What is this dashboard**? It's built on top of airtable. If you didn't know, airtable is part spreadsheet, part database and incredibly smooth and flexible. The best way to understand is to watch their 2min [product tour](https://airtable.com/product)

This dashboard is designed for big user managing 10-100+ accounts. For a simpler version, you can ask us to switch to the classic dashboard.

## How to start?

Alright, lets get a quick overview of airtable.

![Screen Shot 2020-03-24 at 10.53.53 AM.png](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/03/24-10-58-14-Screen%20Shot%202020-03-24%20at%2010.53.53%20AM.png)

So this is your **base**

Your got different **tables** ( the piece of the puzzle ): account, domain ect..

You have **view** which is just a way to show or hide a set of column, so you can focus on current task ( setting up campaign, sceduling etc...). You can create your own view, and customize it for your VA.

### Let's set up your first campaign

1. Start by adding an account.
   
   ![Screen Shot 2020-03-24 at 11.03.17 AM.png](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/03/24-11-03-55-Screen%20Shot%202020-03-24%20at%2011.03.17%20AM.png)
   
   You need to assign a source and a user . Optionnaly you can set up the status which is just to help you organize things ( which account are live, in review etc.. ) and the account pixel.

2. Then you can create your campaign
   
   ![Screen Shot 2020-03-24 at 11.07.15 AM.png](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/03/24-11-08-07-Screen%20Shot%202020-03-24%20at%2011.07.15%20AM.png)
   
   You need to define these:
   
   - the **source** 
   
   - the **account** we just added
   
   - the **flow** ( which vertical, geo and device ?
   
   - the **[integration](#integration)**, which is the kind of safe page you want to use. You either have wordpress ( an article as safe page ) or a reverse proxy ( where you can use any external website as your safe page) more on that later..
   
   - [Domain](#domain). For the domain, if you already have domain available in your base, you can assign manually. If you don't and need a new domain, click on deploy ( this will assign you a new domain based on your settings)
     
     ![Screen Shot 2020-03-24 at 11.10.44 AM.png](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/03/24-11-11-01-Screen%20Shot%202020-03-24%20at%2011.10.44%20AM.png)
     
     That's all. Once you get a domain, you will see your campaign URL. 
     All is ready, you can use it in your traffic source.
     
     ![Screen Shot 2020-03-24 at 11.11.41 AM.png](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/03/24-11-11-46-Screen%20Shot%202020-03-24%20at%2011.11.41%20AM.png)
     
     The last step is to activate your campaign after the traffic source approved it.
     
     ![Screen Shot 2020-03-24 at 11.12.43 AM.png](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/03/24-11-13-06-Screen%20Shot%202020-03-24%20at%2011.12.43%20AM.png)

# Campaign

Deploy a campaign

## Campaign scheduler

Campaign scheduler is a bot that will auto start and auto pause campaign on the time and day you choosed.

It's useful because most of the offers have ON hours where you get most of the traffic and higher CR. Letting campaign live at night increase the risk of getting your campaign banned. Scheduling your campaign reduce risk of getting banned by 50%

![Screen Shot 2020-03-18 at 11.12.20 AM.png](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/03/20-15-49-12-Screen%20Shot%202020-03-18%20at%2011.12.20%20AM.png)

### How it works ?

The timezone is UTC so you need to adjust based on that.

- Ie you launch a campaign in USA from 8h to 20h local time GTM-4 , you need to convert schedule to 12:00 - 24:00
- Ie campaign in Germany from 8h to 20h local time GTM+1 , you need to convert schedule to 7:00 - 19:00

What else to know:

- The scheduler run every 30min, so don't set 9:15 as it will count as 9:30 anyway
- Make sure to tick the box schedule to make the bot active.

# Lander

### How to add safe page

### How to add money page

coming soon

# Offers

### How to add offers

coming soon

#### classic dashboard
