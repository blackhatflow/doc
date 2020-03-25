



# Case study

- **Source** VoluumDSP -> revcontent
- **Vertical** ED
- **Geo** US
- **Network** : blackflow + c5 interactive

*I will go through each step of the process and show everything:*

- Part 1 – create campaign on blackflow
- Part 2 – setting up campaign on voluumdsp
- part 3 – optimize and results

**The results**

- Day 1 : Spend 120, Rev 160, ROI +33%
- Day 2 : Spend 100, Rev 224, ROI +124%

***What is blackflow?*** *Blackflow gives you proven blackhat campaign ready to run. Under the hood, we provide all that’s needed: cloaking, hosting, unique server ips and domains, safe page, lander, and offers. You just have to launch and focus on your traffic*

&nbsp;

---

&nbsp;

**PART 1 – 5min**

# Build your campaign

## Create a campaign on blackflow

- Go to https://app.blackflow.io and create a new campaign

![](https://blog.blackflow.io/wp-content/uploads/2019/11/Screen-Shot-2019-11-26-at-7.46.12-PM-1.png)

- STEP 1 – Select the traffic source and vertical

- STEP 2 – Select the device, country and then click on create campaign

- STEP 3 – copy your campaign link
  
  ![2020-01-16 10.46.02.gif](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/01/16-10-47-48-2020-01-16%2010.46.02.gif)

---

### How your campaign link works?

`https://lifefify.com/?source=voluumdsp&campaign=8541abda&cid={campaign.id}&sid={dsp.widget.id}&aid={dsp.creative.id}&tid={dsp.adexchange}&uid={clickid}`

- On an abstract level, your link looks like this :

    `domain.com/?campaign&tracking&customize`

 

 

- domain
  
  `https://lifefify.com`

    The domain name is unique to your account and we don’t share it we other affiliates.

- campaign

    `?source=voluumdsp&campaign=8541abda`

This is the mandatory part, it’s how we route your traffic to the right funnel

- tracking

    `cid={campaign.id}&sid={dsp.widget.id}&aid={dsp.creative.id}&tid={dsp.adexchange}&clickid={clickid}`

    This is the **tracking** on your traffic source.

    We track 4 parameters so you can optimize it. You will find them on the blackflow stats dashboard.  

| **URL Parameter** | **Stand for**              | **Stats report** |
| ----------------- | -------------------------- | ---------------- |
| cid               | campaign                   | Campaign         |
| sid               | placement / widget / Adset | Placement        |
| aid               | creative / Ad              | Creative         |
| tid               | platform / domain          | Domain           |
| clickid           | clickid (optional )        | Users            |

You can use them the way you want, just map them correctly.

&nbsp;

---

&nbsp;

## Customize your campaign

![](https://blog.blackflow.io/wp-content/uploads/2019/11/Screen-Shot-2019-11-26-at-8.57.16-PM.png)

#### Now let's choose the landers, using url parameters *m=* and *s=*

Blackflow let you choose which lander to show, depending on your angle

Use these parameters in your campaign link:

- **m=xx** ( m for money lander 💰💰💰 )
- **s=xx** ( s for safe lander 😇😇😇) 

to learn more about it [https://help.blackflow.io/en/articles/3373003-customize-the-flow](https://help.blackflow.io/en/articles/3373003-customize-the-flow)

Let’s have a look into the lander library that we get from spytools. There are loaded in the system, you just have to choose.

- **Quality** 👍 is a subjective appreciatiabout how good we think the lander is

- **Compliance** 😇 is about the compliance of the lander. It’s up to you to choose your risk level

- **EPC** 💰 and **Volume** ⚖️ are the stats blackflow wide. So you see exactly **what’s working and what’s hot.** If a lander doesn’t have any stats, it doesn’t necessarily mean it’s bad, we may just have add it or nobody thought of a good angle to run it yet.

So here I choose m=122. If I want to split test I would use m=122,79, and i could even define the rotation weight by using m=122,122,79 ( Lander 122 would get 2/3 of the traffic and 79 would get 1/3 )

For the safe page, i will trust the default rotation that we already tested and that works for voluumdsp ( which is the right balance between getting approved easily AND monetize the traffic ). So i won’t use the param s=

**So my final link is**

`https://lifefify.com/?source=voluumdsp&campaign=8541abda&cid={campaign.id}&sid={dsp.widget.id}&aid={dsp.creative.id}&tid={dsp.adexchange}&uid={clickid}&m=122,79`

&nbsp;

---

---

&nbsp;

**PART 2 – 10min**

# Set up voluumDSP

## Create the campaign

Next is to set the campaign on the traffic source

Not rocket science here, just insert your campaign link

![](https://blog.blackflow.io/wp-content/uploads/2019/11/Screen-Shot-2019-11-24-at-1.46.21-PM.png)

Targeting is Revcontent USA here, but anything works.

![](https://blog.blackflow.io/wp-content/uploads/2019/11/Screen-Shot-2019-11-24-at-1.38.49-PM.png)

Strategy on native traffic source is pretty much the same: Start small and cap the placement at low spend to not get burn and slowly block bad placements

![](https://blog.blackflow.io/wp-content/uploads/2019/11/Screen-Shot-2019-11-24-at-1.38.57-PM.png)

---

&nbsp;

### Creatives

Now the Creative part …

Go on blackflow, in the customize section. We provide images of what works ( these come from spy tools ).  
Of course it’s better if you use your own, we just provide it as sample.

![](https://blog.blackflow.io/wp-content/uploads/2019/11/Screen-Shot-2019-11-26-at-11.34.45-PM.png)

Same note for the headline, you can have a look at our collection, if you don’t feel inspired today.

![](https://blog.blackflow.io/wp-content/uploads/2019/11/Screen-Shot-2019-11-26-at-11.37.17-PM.png)

Let’s keep it simple and select 3 images + 3 headlines.  
Once uploaded in voluumDSP you get 3*3=9 combinations.

---

&nbsp;

### Activate your campaign

Make sure that on voluumDSP your campaign is on pause while they review it.  
After their compliance team approve it, go to blackflow.io/campaign and activate your campaign

![](https://blog.blackflow.io/wp-content/uploads/2019/11/Screen-Shot-2019-11-26-at-11.40.36-PM.png)

This is very important, otherwise all your traffic will be filtered by the cloaker.

---

&nbsp;

### Setting up the pixel

> While Waiting our campaign to get approved, let’s set up the pixel

Blackhat is amazing at tracking your users behavior, so let’s make sure we are sending these data back to the traffic source so we can optimize our traffic cheaper. We are going to fire the pixel for these events:

- **view** : the user see the lander and is tracked ( removing bots )

- **m** : user see the money page

- **10s** : user stay at least 10s ( so we see bad placements that just bounce)

- **30s** :  user 30s

- **60s**

- **120s**

- **180s** : ( starting to show good intent )

- **240s** : ( that’s usually the time they need to read before buying )

- **lead** : ( click + time >60s )

- **sale**
  
  ![Screen Shot 2020-01-16 at 10.07.42 AM.png](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/01/16-10-08-26-Screen%20Shot%202020-01-16%20at%2010.07.42%20AM.png)

![](https://blog.blackflow.io/wp-content/uploads/2019/11/Screen-Shot-2019-11-26-at-3.24.15-PM.png)

And for the **lead** and **sale** event, you want to mark it as a conversion and save the payout

![](https://blog.blackflow.io/wp-content/uploads/2019/11/Screen-Shot-2019-11-26-at-3.24.33-PM.png)

![](https://blog.blackflow.io/wp-content/uploads/2019/11/Screen-Shot-2019-11-26-at-3.27.08-PM.png)

Just send us the pixel for your account, it’s all automated.

---

---

&nbsp;

**PART 3**

# Optimize

> *Results of day 1 – Pretty good ROI +33%*

*So on day 1, we end up spending 120\$ and making 160$  revenue, which is profitable of course, but not that great ( remember it’s blackhat ). That said we are buying native traffic so there is a lot of room for improvement. Being profitable on day 1 is actually a really good sign nowadays.*

### Let’s optimize

We are going to check and optimize three variables:

- the placements aka widget

- the creatives

- the lander ( if you did split testing instead of the default rotation )

---

&nbsp;

### Placements

On voluumDSP you pretty much have all you need already, thanks to the pixel firing for each events.

![Screen Shot 2020-01-16 at 10.06.58 AM.png](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/01/16-10-25-59-Screen%20Shot%202020-01-16%20at%2010.06.58%20AM.png)

![](https://blog.blackflow.io/wp-content/uploads/2019/11/Screen-Shot-2019-11-26-at-6.35.33-PM.png)

*Head to blackflow.io/stats and Let’s look at the placements*

![](https://storage.googleapis.com/blackflow-blog/2019/11/174cb493-screen-shot-2019-11-27-at-2.54.34-pm-1024x518.png)

Cut bad placement after only 10 clicks

What’s good here, **is that we can optimize placements after very few clicks.**

Usually, affiliates optimize on CVR, but’s that’s expensive as you have to spend at least 1-2 times the offer payout before knowing if the widget is good. Here we are promoting nutra ED, the payout is usually 64$, so that’s a very expensive and inefficient strategy.

But now, with blackflow we can just check the time behavior and the leads, which tell us a lot about the traffic quality.

I have a small budget so I’m going to set up strict rules for the beginning:

- If > 5 users, and time 60s < 1 Then block ( Mean that the placement don’t send any real user )
- If >10 users And lead < 1 Then block ( remember we set up a lead as scrolling 50% + staying 60s + click – so we can separate real click with intent from fraudulent clicks )

![](https://blog.blackflow.io/wp-content/uploads/2019/11/Screen-Shot-2019-11-26-at-8.52.57-PM.png)

I actually set up the event – lead as a conversion. So that’s the rule from above

____

&nbsp;

### Creatives

*Next let’s have a look at the creative*

**

![](https://blog.blackflow.io/wp-content/uploads/2019/11/Screen-Shot-2019-11-26-at-3.13.25-PM-2048x871.png)

![](https://storage.googleapis.com/blackflow-blog/2019/11/d2654b5b-screen-shot-2019-11-28-at-8.18.56-pm-1024x164.png)

creative stats on blackflow, easy to compare with duration, scroll %, click time, bounce

Creatives look fine here, I just notice one of the ad got a low CPC so that’s good sign for tomorrow

---

&nbsp;

### Landers

![](https://storage.googleapis.com/blackflow-blog/2019/11/1f6c73af-screen-shot-2019-11-27-at-10.43.36-pm.png)

> BL & WL

For Day 2 I created a white list to focus on the good placements we saw on day 1. The strategy is as usual: Explore placements on the BL and add them to to the WL. On the WL you need to bid a bit higher to get traffic. I added about 15 placements. ( Yes we didn’t get much conversions or data, I selected the widget on the basis of the good behaviors we saw above )

![](https://storage.googleapis.com/blackflow-blog/2019/11/9daf1ea1-screen-shot-2019-11-27-at-12.41.09-am.png)

> Spent 100\$, made 220\$, ROI +124%

![](https://storage.googleapis.com/blackflow-blog/2019/11/925cbde8-screen-shot-2019-11-27-at-12.14.28-am.png)

Revenue on DSP only show 4 conv and 120\$ because we didn’t fire the upsell back. Real revenue is 224$

![](https://storage.googleapis.com/blackflow-blog/2019/11/c1604e98-screen-shot-2019-11-27-at-12.15.01-am.png)

> let’s check the lander, see if we can make anything better

![](https://storage.googleapis.com/blackflow-blog/2019/11/5966a348-screen-shot-2019-11-27-at-3.00.55-pm-1024x519.png)

Go the blackflow.io/stats in the lander reports

![](https://storage.googleapis.com/blackflow-blog/2019/11/b302da2c-screen-shot-2019-11-27-at-3.01.15-pm.png)

It’s a bit early to optimize here, but we see our lander are both working well.

On blackflow we already cleaned and tested the landers for you, so we protects your bottom line. 

____

[Click here to get started](https://app.blackflow.io/signup)

thank you for reading, until next case study.
