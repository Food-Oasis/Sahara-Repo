# Sahara-Repo
This repo is devoted to development of aspects of the Food Oasis application which Team Sahara is responsible for.

## Connecting to the GCP MySQL Instance
There are several ways to connect to the MySQL instance but the simplest way is using GCP. If you are looking for the original database intialization file, you can follow [this link](https://github.com/Food-Oasis/Sahara-Repo/MySQL_Database/FoodOasisSQL.sql)

### Activating your Google Cloud Console
To connect to our instance you must open you [Google Cloud Platform console](https://console.cloud.google.com/?_ga=2.121883787.-1085226358.1566396986) associated with you Google Account. Once you are connected you should click the button in thr top right conner pictured below:

![button](https://github.com/Food-Oasis/Sahara-Repo/MySQL_Database/activate.PNG)

In the balck termninal that arises copy and paste the following line:

`gcloud sql connect food-oasis-database --user=root --quiet --project="food-oasis-database"`

When prompted for the password simply press enter and you will be logged into the root user. To navigate into the Food Oasis database, run the following lines:

`USE FOOD_OASIS;`
`SHOW TABLES;`