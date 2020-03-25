faq

# Frequent questions

#### How is blackflow different from other all-in-one tools like zeustrack or kowboykit.

Blackflow is similar in the way that we bring the piece of the puzzle together ( tracking, cloaking, server, safe page etc..)

But the big difference is that we provide **specific knowledge**. All the other service are just a tool-kit where you still have everything to do and test by yourself. Now at Blackflow, we test things, make it work and then we run it the **way we think is best**. And we give no alternative about that. Ie "*for FB what's working is this safe page, plus this setup, using this...* "

#### So how do you know if blackflow is the right choice for your team?

Well if you have a big team, already running things your own way successfully, then we are probably not the best choice.

But for every other case, wether you are running already but you are struggling to scale or just starting to run traffic, and you want a 100% proven method to run a campaign, then Blackflow is definitely the right choice. We give you a campaign link, that you will use on your traffic source and it will works right away. What's left is to optimize it.

### The way I'm defining safe page with &s={id} parameter, do I have to define money page as well similarly? If I want it go to a certain money page and certain offer

 Campaign come with a default funnel. Optionnaly you might want to customize it, using parameter in your campaign link.

- change the safe page with s={pageid} This is highly recommended to change it as you want to match the safe page with your angle, to improve your quality score and get approved by reviewers.

- change the money page with m={pageid} . By default we run the lander that works best, so you don't have to change, unless you run a specific angle, that you know works better with a given lander ( celeb ect... )

- change the offer with o={offerid}. Again this is better to not change it, as we have all the data about what work best and we do optimization already. The only case you want to change it is that you want to work with a specific network/advertiser ( or you own offers ) 

***How can I check which offer is what going to? is it automated or manual I mean the offer selection***

It's automated. You might change it only if you want to work with specific network/advertiser/broker ( or you own offers ).

You can see i which partners we monetized your traffic with in your stats.

***If I'm tracking traffic via voluum how about the postback and stuff where to put/get that from? ***

You don't need to use voluum as 1) we have better analytics, and 2) voluum would add a redirect in the funnel. ( Not concerning voluumDSP ).  blackflow = cloaker + funnel + analytics

***How about pixel data I read your earlier tutorial you can to optimise it quicker you can fire certain pixel events from safe page***

We fire event on money page. We support pixel for voluumDSP, Facebook, Google, Mgid. 

#### so it must be super slow via 3 cloakers

No, we use api and it's extremely fast. Blackflow filter is on same server and check take 2-5ms, leadcloak take 100-150ms with API and TA a bit slower 300-400ms. In total less than 500ms, that is 2-3x faster than any other cloaker/tracker

##### How can i check if the campaign is working

You can debug everything by adding parameter in your campaign URL.

- you can see click in realtime by adding &{pubid}=log at the end of your link. ( replace {pubid} by you pubid. Example, my pubid id is ab, so ab=log ) 
  https://pauluma.com/?source=googleads&campaign=7e3fe4w8f6x&ab=log

- you can see cloaker response using ab=cloaker

- you can see traffic armor response using ab=trafficarmor

- you can see output ( money page / safe page ) ab=output

- you can bypass cloaker ab=bypass

ss

Should i pause my campaign on blackflow when my traffic is not live ?

Yes, absolutely. Even if we cloak all traffic, it's not 100% bullet proof. So we highly recommend that if you do advertise on fb / google, you pause your campaign on blackflow during off-hours ( ie for crypto, no reason to be live at night, CR is low anyway, so pause it. Your account will last twice longer )
