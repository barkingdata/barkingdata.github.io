---
layout: post
title: Etsy Top Selling Shops With Time Series!
---


Etsy, Inc. an American e-commerce company focused on handmade or vintage items and craft supplies. These items fall under a wide range of categories, including jewelry, bags, clothing, home décor and furniture, toys, art, as well as craft supplies and tool. There are millions of transactions being generated on the entire platoform. We are interested to get some understanding about how many sales are genrated over some fixed tiem intervals and who are the top performing shops in temrs of sales volume. We are also interested in which shops are are the most liked or followed shops, and how many customer reviews they receive. 

However, to address the above questions is definitely not an easy task. Luckily, with our modern AI based web technology, we are able to track and monitor the most active shops on the platform on weekly or monthly basis frequency.


As briefly mentioned here already, [https://barkingdata.com/?etsy-top-shops/]
Now let's take a more closer look at what and how we can track and extract from the shops. First, let's open a random shop's profile page, please note that this page is a public page and can be accessed by any ordinary PC desktop or mobile device user.

![image](https://user-images.githubusercontent.com/105116671/167261344-c5bf326d-a501-4e3c-b4fc-060942a8337d.png)

Let's scrape some public info about the shop such as total sales, total likes, review count, ratings etc. and store these data atrributes into a relational database such as MySQL/Sybase/Oracle etc, then repeate the scrape for the other shops as well! Since the purpose of this blog is to demonstrate what we can do with the data, we are not going to talk about too much about the data collection process. 

After a week or two, we come back to extract the data again and we will have two rounds of data in the database. Now lets' start the data processing part. First, we use internal tools to clean up the raw data a little bit to make it better quality for the subsequent analytics part. After cleaning up, we then use some python script to calculate the sales volume difference between the two rounds of raw data. Lastly, we use business intelligence and data visualization tools to apply the final analysis and aggreation to the dataset and plot some charts. 

The chart below gives a clear picture of the top selling shops between the two rounds of data collection.

![image](https://user-images.githubusercontent.com/105116671/167260550-6217b290-71cc-410c-9739-0ed1348d7212.png)

Also in the raw data we can collect the shop create date for each shop. We can also easily make a plot for shops create date.

![image](https://user-images.githubusercontent.com/105116671/167261893-fb513c9f-78e3-4652-80f6-32e545923af4.png)

We can get a pretty clear picture of how new shops get created on the platform over time. From the chart above , it telsl us that in 2020 when Covid started, the number of new shops also went up quite a bit during the year of the pandemic started.

Similarly, we can also plot more charts for other metrics. I shared some top selling shops to download for free, please download from here:
https://www.kaggle.com/datasets/polartech/1m-etsy-shops-sales-data 
