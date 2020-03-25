## GoogleAds Pixel

### setting up the pixel

We will set up : 

- **[Lead](#Lead)** : it will fire automatically from your campaign

- Check if the google [auto-tagging glcid](#gclid) is active 

### 1) **Lead** :

 *will fire automatically from the lander, when we detect the click to offer is good quality ( time on page > 120s + scroll +50%. )* **Avg Lead to Offer Lead is 50%**

![Screen Shot 2020-01-23 at 4.04.27 PM.png](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/01/23-16-07-24-Screen%20Shot%202020-01-23%20at%204.04.27%20PM.png)

![Screen Shot 2020-01-23 at 4.00.08 PM.png](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/01/23-16-08-12-Screen%20Shot%202020-01-23%20at%204.00.08%20PM.png)

1. Choose Website

2. keep note of the ***conversion ID*** ( associated to your googleads account ) and ***conversion Label*** ( specific to that conversion event )

3. Set up pixel on blackflow: On your ad account on blackflow, enter this as pixel :

    `{conversion ID}-{Conversion Label}`

     in this example, it looks like this:

    `685124755-iAofCJ_D2LcBEJPZ2MYC`

Then you either:

- send to us to put in globally on your account 

- or, in your campaign link use parameter &pid={pixelid} like this &pid=685124755-iAofCJ_D2LcBEJPZ2MYC

#### gclid

Very important: you need to activate google auto tagging, the gclid, because 1) if not your traffic will be filtered and 2) you can use it for pixel

![Screen Shot 20200127 at 92626 PMpng](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/01/27-21-26-29-Screen%20Shot%202020-01-27%20at%209.26.26%20PM.png)

![Screen Shot 2020-02-20 at 2.16.00 PM.png](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/02/20-14-20-44-Screen%20Shot%202020-02-20%20at%202.16.00%20PM.png)
