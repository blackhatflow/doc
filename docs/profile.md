# profile

## pubid / pubkey

You will need your pubid and pubkey. You can find them in settings -&gt; profile.

![Screen Shot 2020-01-04 at 10.44.48 AM.png](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/03/30-16-02-18-Screen%20Shot%202020-01-04%20at%2010.44.48%20AM.png)

* Your pubid is generated from your name to make it easy to remember.
* Your pubkey, is your secret key that allow you to debug your campaign.

  By default pubkey = pubid but we highly recommend to change it once you have real traffic.

  Otherwise, if someone see a campaign xxxxxxx and somehow guess it belong to you, could try to bruteforce \( find your two letter pubid by trying randomly \) and then see your stats. Even then, it's a small leak as the stats available from the campaign link are limited.

## Debugging your campaign link

In your campaign link you can use:

* **&pubkey=cloaker** _to see the cloaker response_
* **&pubkey=flow** to see the funnel configuration
* **&pubkey=log** _to see in realtime the last 100 clicks_
* **&pubkey=stats** \*to access the campaign stats in standalone mode \( stats are updated every hours \). Useful to give stats access on campaign level to your VA or partner without sharing your login

