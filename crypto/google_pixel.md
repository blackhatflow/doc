# GoogleAds Pixel

## setting up the pixel

We will set up two conversions :

* [**Lead**](google_pixel.md#Lead) : it will fire automatically from our **Website**
* [**Purchase**](google_pixel.md#Purchase) : you will **import manually** the conv later on \( we can't fire pixel for ftd or offer lead for now \)

  ![Screen Shot 2020-01-23 at 4.06.15 PM.png](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/01/23-16-09-21-Screen%20Shot%202020-01-23%20at%204.06.15%20PM.png)

## 1\) **Lead** :

_will fire automatically from the lander, when we detect the click to offer is good quality \( time on page &gt; 120s + scroll +50%. \)_ **Avg Lead to Offer Lead is 50%**

![Screen Shot 2020-01-23 at 4.04.27 PM.png](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/01/23-16-07-24-Screen%20Shot%202020-01-23%20at%204.04.27%20PM.png)

![Screen Shot 2020-01-23 at 4.00.08 PM.png](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/01/23-16-08-12-Screen%20Shot%202020-01-23%20at%204.00.08%20PM.png)

1. Choose Website
2. keep note of the _**conversion ID**_ \( associated to your googleads account \) and _**conversion Label**_ \( specific to that conversion event \)
3. Set up pixel on blackflow: On your ad account on blackflow, enter this as pixel :

   `{conversion ID}-{Conversion Label}`

   in this example, it looks like this:

   `685124755-iAofCJ_D2LcBEJPZ2MYC`

## 2\) **Purchase**

we will import them manually in case of FTD \( first time deposit \). We don't need any conversion ID here, but the name _**conv**_ matter!

![Screen Shot 2020-01-23 at 4.05.27 PM.png](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/01/23-16-07-17-Screen%20Shot%202020-01-23%20at%204.05.27%20PM.png)

![Screen Shot 2020-01-23 at 4.04.39 PM.png](https://raw.githubusercontent.com/blackhatflow/storage/master/2020/01/23-16-08-04-Screen%20Shot%202020-01-23%20at%204.04.39%20PM.png)

