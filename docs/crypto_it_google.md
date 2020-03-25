# Crypto Italy + Google Adword

This case study is about launching campaigns on Google AdWords, promoting crypto in Italy.

As it's one of the first case studies, I will details each step a bit more and keep it updated.

CONTENT

1. Intro and mindset

2. make your [campaign link](#campaign) and safe page

3. Set up the pixel](#pixel). and activate auto-tagging gclid ( google click id)

4. [build the ad](#ad) and set up the campaign on AdWords

5. Then [optimize](#optimize) and see our [tips](#tips)

# Intro

So google search and their partners are very good quality. And it's about getting the right intent (keyword) to your campaign.

About account, it seems that your account either get banned in the first few days ( account quality issue or your ad copy is too aggressive and don't make sense ) or it last very long 3weeks+ . For extra safety, you need to pause your campaign on blackflow during off-hours so all the traffic is filtered with 0 fingerprint

![Screen Shot 20200123 at 80508 PMpng](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/01/23-20-05-17-Screen%20Shot%202020-01-23%20at%208.05.08%20PM.png)

The mindset to have on crypto is to focus on a smaller metric than FTD. Reaching stats significance on FTD is very hard as the value is high $700+ . so most of the time it's difficult to reach a conclusion and is mostly random. It's a combination of time of the day, if the client is available, which broker is calling etc...

So you want to focus on Lead ( click that have high chance to convert ) and offer conversion ( user filling information on offer page ). Then you trust the broker and overall the conv to FTD rate is 10% . That means on some day you can make 10 conv and no conversion and the next day make 2 conv and 2 ftd.. Just saying so you don't freak out and force yourself to see a bit long term. Also, google is optimizing slowly so don't keep changing things (lander/keyword) all the time. Set it up and let it alone. The less you touch settings the better. If you want to make a big change ( new geo, new domain ), please iterate by launching a new campaign on new account.

Also, about 20-30% of the FTD happen days later. ( The reason is that the call center is calling again and pushing the client to make the deposit ).

So again: Don't freak out, trust the stats, and focus on your cost per conv.
And another rule: When campaign is good, don't touch anything, just let it run. Only slowly increase budget while keeping under 1k/d

# campaign

So creating a campaign on blackflow, you get a link looking like this :

```
https://domain.com/?source=googleads&campaign=68449c63&cid={campaignid}&sid={keyword}&aid={creative}&tid={target}
```

This link is all ready, you might want to change the safe page and money page to match your angle.

#### Choose money and safe page ( optional )

this is optional, if the safe page by default don't match your ad angle, then:

1. use m={id} in your campaign link ( m stand for Money page)

![](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/01/16-20-53-52-Screen%20Shot%202020-01-16%20at%208.53.04%20PM.png)so if you choose to show safe page "safe work from home" i will use s=276

**Quick note about the domain. ** Things are changing fast, so I currently do things manually instead of systemizing and adding to your dashboard. Currently, you either get a domain with a Wordpress or a now.sh with reverse proxy. Just ask

# pixel

We will set up :

- **[Lead](#Lead)** : it will fire automatically from your campaign

- Check if the google [auto-tagging glcid](#gclid) is active

### **Lead** :

*will fire automatically from the lander, when we detect the click to offer is good quality ( time on page > 120s + scroll +50%. )*  **Avg Lead to Offer Lead is 50%**

![Screen Shot 20200123 at 40427 PMpng](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/01/23-16-07-24-Screen%20Shot%202020-01-23%20at%204.04.27%20PM.png)

![Screen Shot 20200123 at 40008 PMpng](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/01/23-16-08-12-Screen%20Shot%202020-01-23%20at%204.00.08%20PM.png)

1. Choose Website

2. keep note of the ***conversion ID*** ( associated to your google ads account ) and ***conversion Label*** ( specific to that conversion event )

3. Set up pixel on blackflow: On your ad account on blackflow, enter this as pixel :

`{conversion ID}-{Conversion Label}`

     in this example, it looks like this:

`685124755-iAofCJ_D2LcBEJPZ2MYC`

Then you either:

- send to us to put in globally on your account

- or, in your campaign link use parameter &pid={pixelid} like this &pid=685124755-iAofCJ_D2LcBEJPZ2MYC

#### gclid

**Very important:** you need to activate google auto-tagging, the gclid, because

1. if not your traffic will be filtered

2. you nee it in order to use the pixel

![Screen Shot 20200127 at 92626 PMpng](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/01/27-21-26-29-Screen%20Shot%202020-01-27%20at%209.26.26%20PM.png)

![Screen Shot 20200220 at 21600 PMpng](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/02/20-14-17-46-Screen%20Shot%202020-02-20%20at%202.16.00%20PM.png)

---

# Ad

Let's set up the campaign on adwords. In our example, we use the "make money online" angle

Quick tip to translate your keyword across campaign.

Translation ( you can use google sheet to translate easily with this formula =GOOGLETRANSLATE({texttotranslate},"en","it")

| EN                               | IT                                                |
| -------------------------------- | ------------------------------------------------- |
| make extra money online          | fare soldi extra online                           |
| make money online from home.     | fare soldi online da casa.                        |
| best online job for salary. easy | miglior lavoro online per stipendio extra. facile |
| earn money online from home      | fare soldi extra online da casa                   |

### keyword

you can try some exact match and broad keyword, that you can later optimize.

fare soldi da casa
fare soldi online
come fare soldi
come guadagnare denaro extra
come guadagnare soldi da casa

## setup

Google strategy is entirely up to you, but here are our settings anyway.

We want to set up the right campaign right away. That means put your real targeting, real ad copy from the beginning. Again, to each his own, but for us, it makes no sense to warm up an account on a totally different campaign then switch and start over.
What we do is set up the real campaign and let it spend while the campaign is OFF on blackflow. Then after a few days, we turn it on and we don't change anything on google ads. The only thing we touch is the budget.

At first we will optimize our campaign for clicks.. then after we get enough conversion ( spend 200+ ) we switch to CPA optimization ( google will suggest to switch to CPA optimization after 10 conv per ad or so)

While optimizing for click, we want the most traffic we can while limiting the CPC ( or you could have bad surprise ). No rules here but no point in paying >1.5 per click for warming up and getting data. 0.5-1.5 is a good range.

So first, let's make a campaign with :

- traffic as objective

- search + google partners

![Screen Shot 20200123 at 93943 AMpng](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/01/23-09-40-16-Screen%20Shot%202020-01-23%20at%209.39.43%20AM.png)

- location Italy

- Language Italian

![Screen Shot 20200123 at 94042 AMpng](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/01/23-09-42-58-Screen%20Shot%202020-01-23%20at%209.40.42%20AM.png)

Then we want to schedule our campaign to run every day during working hours and weekdays. So we don't have to log in to account and pause/activate later on.

The best hours for CVR seems to be 8 am-4 pm local time. It convert less as night ( call center are closed and won't call your leads ), and convert less on weekend ( people don't answer the phone so much ).

Here I make it start a bit before 7am to get some momentum at 8am

![Screen Shot 20200123 at 94212 AMpng](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/01/23-09-42-44-Screen%20Shot%202020-01-23%20at%209.42.12%20AM.png)

I will warm up the campaign with a low budget for the first few days. ( Duration depend to you, and your account quality)

![Screen Shot 20200123 at 94219 AMpng](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/01/23-09-42-40-Screen%20Shot%202020-01-23%20at%209.42.19%20AM.png)

![Screen Shot 20200123 at 92737 AMpng](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/01/23-09-27-46-Screen%20Shot%202020-01-23%20at%209.27.37%20AM.png)

![Screen Shot 20200123 at 94608 AMpng](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/01/23-09-46-18-Screen%20Shot%202020-01-23%20at%209.46.08%20AM.png)

![Screen Shot 20200123 at 94710 AMpng](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/01/23-09-47-21-Screen%20Shot%202020-01-23%20at%209.47.10%20AM.png)
Other settings that i'm setting up for this campaign ( it's optional and depends of your angle )

Exclude mobile traffic by setting the bid to -100%

![Screen Shot 2020-03-10 at 3.12.10 PM.png](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/03/10-15-16-13-Screen%20Shot%202020-03-10%20at%203.12.10%20PM.png)

Exclude age 18-34

![Screen Shot 2020-03-10 at 3.13.15 PM.png](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/03/10-15-15-46-Screen%20Shot%202020-03-10%20at%203.13.15%20PM.png)

You can also only target a gender ( i won't do in this campaign )


---

## optimize

after a few days, you will get enough conv ( ideally > 10-15 ) to optimize for CPA.. and this is where the magic happens.

Then a good cost per conv is 20-30.. you don't want to scale if your cost per conv is higher than 40..

Most converting device is desktop so you need to factor that as well. For mobile/tablet cost per conv should be below 25 to beak even

![Screen Shot 20200220 at 25640 PMpng](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/02/20-14-57-36-Screen%20Shot%202020-02-20%20at%202.56.40%20PM.png)

Set up the target CPA recommended by google or set it up manually higher to get more traffic. You might need to adjust based on results and spend.

![Screen Shot 20200220 at 25628 PMpng](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/02/20-14-58-12-Screen%20Shot%202020-02-20%20at%202.56.28%20PM.png)

