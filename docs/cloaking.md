[blackflow.io](https://blackflow.io)

# Guide to cloaking

*Blackflow take care of the cloaking and integration, but sometimes, you need to choose the cloaking method yourself, as it depends on your angle. Just ask us if you have doubt.*

*What blackflow do for you in the backend:*![Screen Shot 2020-01-21 at 10.17.04 AM.png](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/01/21-10-17-40-Screen%20Shot%202020-01-21%20at%2010.17.04%20AM.png)

## How to choose a cloaking method

#### Blackflow currently have 5 options for the safe page

- **[redirect](#redirect)**: redirect to any page like amazon, ebay etc.. 

- **[curl](#curl):**: host any external page ( but it's not a mirror - if you click links on the page it will go to original site) 

- **[reverse proxy](#reverse-proxy)**:: fully mirror an external site, we only support a few domain ( etsy, usatoday, euronews etc.. )

- **[wordpress](#wordpress)**: arbitrage website with wordpress, top 10 article, next button and display ads

- **[includes](#includes):**: best scenario where we host a custom lander.

| method            | same domain | zero -redirect | full website                                |
|:-----------------:|:-----------:|:--------------:|:-------------------------------------------:|
| **redirect**      | no          | no             | ✔                                           |
| **curl**          | ✔           | ✔              | yes, but click links go to original website |
| **reverse proxy** | ✔           | ✔              | ✔ but no SEO authority                      |
| **WP website**    | ✔           | ✔              | ✔ but no SEO authority                      |
| **includes**      | ✔           | ✔              | no ( just a single page lander)             |

&nbsp;

The choice of the methods depends on your **angle** and on the **traffic source.**

#### **<u>here are our current observations</u>**

**facebook** ( Recommendation : Redirect )

*Facebook usually requires a full website with terms and quality content, so **include** is usually not an option, and **wordpress websites** are seeing a lot of disapproval lately.*

| Rank | Method         | Chance of approval | Spending |
| ---- | -------------- | ------------------ | -------- |
| 1    | **redirect**   | 9                  | 6        |
| 2    | reverse proxy  | 8                  | ?        |
| 3    | curl           | 7                  | ?        |
| 4    | shopify/github | 8                  | 5        |
| 5    | WP             | 3                  | 3        |

**google** ( Recommendation : WP website )

| Rank | Method        | Chance of approval | Spending |
| ---- | ------------- | ------------------ | -------- |
| 1    | WP website    | 9                  | 9        |
| 2    | reverse proxy | ?                  | ?        |
| 3    | curl          | ?                  | ?        |
|      | ~~redirect~~  | 0                  |          |

**native** ( Recommendation : curl  / reverse proxy )

| Rank | Method        | Chance of approval | Spending |
| ---- | ------------- | ------------------ | -------- |
| 1    | WP website    | 8                  | 10       |
| 2    | redirect      | 9                  | 9        |
| 3    | reverse proxy | ?                  | ?        |
| 4    | curl          | ?                  | ?        |

&nbsp;

---

&nbsp;

## How to use it

let's go over the methods and how to use it

### wordpress

Attached to your domain is a content website ( WP ) with random article. It looks similar to an arbitrage website with clickbait article, 'next >' button and ads.

This is a good option for source that tolerate arbitrage ( taboola, revcontent etc ... not so much for facebook anymore). Another issue is that most of the farming company were using this method, so it's a bit burned.

it allow you to choose a safe page with an article congruent to your angle

Let's try it.

![Screen Shot 2020-01-17 at 3.20.22 PM.png](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/01/17-15-22-42-Screen%20Shot%202020-01-17%20at%203.20.22%20PM.png)

Lander > Filter by integration

![Screen Shot 2020-01-17 at 3.23.30 PM.png](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/01/17-15-23-34-Screen%20Shot%202020-01-17%20at%203.23.30%20PM.png)

For example for crypto IT, we have loaded articles about* 'top works to do from home*' or '*richest people*' or *'investment tips*' . The point is that it's **congruent** to any angle you can think of for your ad. ( Congruent = it will make sense when the source check your funnel ). 

[https://www.lifefify.com/rec0wE8mpDC13DRlv/](https://www.lifefify.com/rec0wE8mpDC13DRlv/)

Note : If you need an article we don't have yet, just ask us.

&nbsp;

### Redirect

*the **redirect** method simply redirect the user to another website. Some source like Googleads don't allow it, facebook is fine with it (lately), and native source can't really ban it as there is still many agencies using a tracking link.*

Here is a very simple ( and plain stupid ) example with amazon.

Let's go on amazon.com ( or amazon.it, .de, .fr etc.. ) and pick any product that you think make senses for your ad. 

![](/Users/yoann/Documents/blackflow/frontend/casestudy/2020-01-17-15-42-49-image.png)

The way to use is very simple: **add the path of the safe page to your campaign link.**

To explain step by step:

- Get the URL

```
https://www.amazon.com/Rise-Bitcoin/dp/B00XVJ3OB4/ref=sr_1_1?keywords=bitcoin+rise&qid=1576004004&sr=8-1
```

- remove the query part ( after "?" ) and keep only the path:

```
Rise-Bitcoin/dp/B00XVJ3OB4/
```

- insert the path in your campaign link ( after the **.com** and before the **?**)

```html
https://dailable.com/Rise-Bitcoin/dp/B00XVJ3OB4/?source=facebook&campaign=094545a1&cid={{campaign.name}}&sid={{adset.name}}&aid={{ad.name}}
```

- Last, append the safe page parameter (s=), so we know which domain to redirect to. 
  
  Here we want to redirect to amazon.it, the ID is 304, so we will add **s=304**
  
  ![Screen Shot 2020-01-17 at 3.51.41 PM.png](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/01/17-15-51-45-Screen%20Shot%202020-01-17%20at%203.51.41%20PM.png)

```
https://dailable.com/Rise-Bitcoin/dp/B00XVJ3OB4/?source=facebook&campaign=094545a1&cid={{campaign.name}}&sid={{adset.name}}&aid={{ad.name}}&s=304
```

And unlike other tracker or cloaker, the redirection is blazing fast ( 135 ms )

![Screen Shot 2020-01-17 at 3.58.40 PM.png](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/01/17-15-58-45-Screen%20Shot%202020-01-17%20at%203.58.40%20PM.png)

&nbsp;

### CURL

with curl method, you can host any external page.

**Example**

1) Choose any page you like. 

https://www.consigli.it/massimo-boldi-e-christian-de-sica-i-film-imperdibili-della-coppia/

2) Load it to blackflow

![2020-01-17 16.32.24.gif](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/01/17-16-32-49-2020-01-17%2016.32.24.gif)

3) Find the ID of the lander you added ( 321 ) and use in safe page parameter **s=321**

![Screen Shot 2020-01-17 at 4.33.41 PM.png](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/01/17-16-33-45-Screen%20Shot%202020-01-17%20at%204.33.41%20PM.png)

&nbsp;

### Reverse-proxy

Reverse proxy method is the **same as curl but in better** , as we create a mirror of the website on our domain. 

With is method, you don't need to load the lander in our system first. You can choose any page of the site. 

( *NOTE: fow now there is still one manual step, you need to tell us which website you want to use so we attach it to your domain* )

**For example**

we want to use this website : [https://www.livemomentous.com/](https://www.livemomentous.com/) It would work well as a safe page for nutra health ( diet, muscle, ed )

On our domain : [https://www.ifadlabs.com/](https://www.ifadlabs.com/)

Then same method as the redirect, you choose any page and copy its path

```
https://livemomentous.com/products/absolutezero-plant?variant=8097396621410

only keep the path : ==> 

products/absolutezero-plant
```

insert that path in your campaign link :

https://ifadlabs.com/***products/absolutezero-plant***?variant=8097396621410&campaign=094545a1

```

https://ifadlabs.com/?source=facebook&campaign=094545a1 

===> 

https://ifadlabs.com/products/absolutezero-plant?variant=8097396621410&campaign=094545a1
```

add the safe page parameter **s=300** ( 300 is the ID for reverse proxy )

```
https://ifadlabs.com/products/absolutezero-plant/?campaign=094545a1&s=300
```

*Note: i removed above the tracking for the explanation, but don't forget to add it*

<u>Our final campaign link for facebook : </u>

```
https://ifadlabs.com/products/absolutezero-plant/?source=facebook&campaign=094545a1&cid={{campaign.name}}&sid={{adset.name}}&aid={{ad.name}}&s=300
```

&nbsp;

### Includes

As the name say, the include method includes the page code. It's normal hosting and it's what most of the cloaker do. The requirement is you own the code of the page, so that's seriously limit your options.s

Just use the ID of the lander s={LanderID}
