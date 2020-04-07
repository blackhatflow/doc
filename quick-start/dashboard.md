---
description: How to use the dashboard
---

# Dashboard

{% hint style="info" %}
**What is this dashboard**? It's built on top of airtable. Airtable is an hybrid spreadsheet and database. If you are new to airtable, watch their 2min [product tour](https://airtable.com/product)
{% endhint %}

## Getting started

Let's get a quick overview of airtable.

![Your dashboard on airtable](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/03/24-10-58-14-Screen%20Shot%202020-03-24%20at%2010.53.53%20AM.png)

* This is your **base**
* You've got different **tables.** See it as ****the pieces of the puzzle : account, domain, landers...
* Then you have **views,** which is a way to filter which columns you want to see, so you can focus on your current task \( setting up campaign, scheduling...\). You can also share a view to your VA \( more on that later \)

### Setting up your first campaign

#### STEP 1 - Add an account.

You start by adding an account. Go to account table.

You need to assign a source and a user . Optionally you can set up the **status** which is just to help you organize things \( which account are live, in review etc.. \) and the account pixel.

![account table](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/03/24-11-03-55-Screen%20Shot%202020-03-24%20at%2011.03.17%20AM.png)



#### STEP 2 - Then you can create your campaign

Go to campaign table

![Screen Shot 2020-03-24 at 11.07.15 AM.png](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/03/24-11-08-07-Screen%20Shot%202020-03-24%20at%2011.07.15%20AM.png)

You can see it as a puzzle, and you need to set these:

* the **traffic source**
* the **account** \(we just added\)
* the **flow** \( which vertical, geo and device \)
* the [**integration**](dashboard.md#integration), which is the type of safe page you want to use. You either have:
  *  wordpress, an article as safe page 
  *  reverse proxy, where you can use any external website as your safe page \( more on that later..\)
* **Domain**. For the domain, if you already have domain available in your base, you can assign them manually. If you need a new domain, click on the deploy, this will assign you a new domain based on your safe page settings

{% hint style="info" %}
Don't see the deploy button? On the right side, click on BLOCKS to show the right side panel, then select the Campaign Dashboard.
{% endhint %}

![](../.gitbook/assets/screen-shot-2020-04-07-at-10.07.30-am.png)

That's all. Once you get a domain, you will see your campaign URL. All is ready, you can use it in your traffic source.

![your campaigns](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/03/24-11-11-46-Screen%20Shot%202020-03-24%20at%2011.11.41%20AM.png)



### Activating your campaign 

The last step is to activate your campaign after the traffic source approved it.

![tick the box on active column](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/03/24-11-13-06-Screen%20Shot%202020-03-24%20at%2011.12.43%20AM.png)

## Manage your Campaign

### Campaign status

A good way to manage your campaign and accounts and to remember what's going on is to set the status of the campaign. This has no effect on the cloaker, it's just for organization. 

{% hint style="info" %}
What if your campaign didn't approved or get banned? Then set up your campaign status as **disabled** and in notes you can indicate the reason. This is very helpful as i can understand why you got banned and make improvements.
{% endhint %}

![](../.gitbook/assets/screen-shot-2020-04-07-at-9.04.00-am%20%281%29.png)

### Campaign scheduler

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

## Landers

### How to add safe page

![Screen Shot 2020-03-24 at 7.35.35 PM.png](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/03/25-15-24-00-Screen%20Shot%202020-03-24%20at%207.35.35%20PM.png)

### How to add money page

_coming soon. for now send over chat_

## Offers

### How to add offers

_coming soon. for now send over chat_

## Collaboration

### Launch sheet

Airtable make it super easy to make launch sheet for your VA

Let's say your VA name is VA1

1. write \[va1\] in campaign notes _\( or on account notes, if you want to share on account level \)_

   ![](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/03/31-10-32-58-Screen%20Shot%202020-03-31%20at%2010.28.57%20AM.png)

2. in campaign table, create a **view** 
   1. name : va1
   2. filter : **notes** contain **\[va1\]** _\( or **account notes** contain **\[va1\]** \)_

      ![Screen Shot 2020-03-31 at 10.39.43 AM.png](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/03/31-10-39-49-Screen%20Shot%202020-03-31%20at%2010.39.43%20AM.png)

   3. show : only the column needed : url, notes, campaign name, account notes etc...

      ![Screen Shot 2020-03-31 at 10.39.05 AM.png](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/03/31-10-39-17-Screen%20Shot%202020-03-31%20at%2010.39.05%20AM.png)

   4. share the view with your VA, optionally you can protect the view with a password

      ![Screen Shot 2020-03-31 at 10.40.21 AM.png](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/03/31-10-40-50-Screen%20Shot%202020-03-31%20at%2010.40.21%20AM.png)

### Ad spend

You want your VA to report the spending per account per campaign. Ideally we would do this from the API but since accounts generally have short live span and using API leave fingerprint, you have to report manually. \( Could make it work with email report that fb send like Kowboykit if you need \)

1. Share the ad spend form with your VA
2. VA fill spend per campaign per day

The spend will show in the stats and will show CPC, CPL, ROI, SPEND

