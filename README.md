# PPKM Analysis From Twitter

This is my academic project in Social Media Analysis with some modification. I get data tweet from this link [PPKM Data](https://drive.google.com/file/d/1JkgBiimNoxGRzgjhQv6gBQpLSTsC1ipK/view?usp=sharing). This data is tweet from January - October 2021 with tweets containing word 'PPKM'.
<br/>
Goals : <br/>
1. Get the pro and cons gender proportion about PPKM
2. Know who is the main source cons stance in PPKM
3. How the pro stance community looks like
<br/>
Note : <br/>
1. This analysis accuration maybe low, because I am not calculate the error
2. Data tweet is not clear enough, there is still business account and maybe a tweet contain 'PPKM' but not really talking about it
3. There is a lot of interpretation about PPKM data, so it will be update it
<br/>

## Step 1 - User Data Collection

Collecting important data for analysis, like username twitter, real name, user name reply and tweet. In this step, I separate data from bot account, business account and real person account with simple methodology. For bot detection, I filter account that has less 1000 followers, not has description and location. Bot account has a tendency characteristics like that. And for business account detection, I filter account has user url that maybe direct to their business url. <br/>

After that, I separate data to user data and tweet text data. User data is used to predict gender account twitter and tweet text data is used to predict stance about PPKM, is it pro or cons about PPKM. <br/>

Before move to step 2 and 3, I annotated data for gender and stance predictioin. In gender prediction, I annotated 100 man and 100 woman. And in stance prediction, I annotated 100 pro and 100 cons.

## Step 2 - Gender Prediction
The prediction is using user real name. If the account doesn't contain real name then using username account. From real name, sometimes we can know the universal gender for that name. So the idea is to chopping real name to some chunks word using char-gram and with machine learning algorithm gender can be detected from training data. 

## Step 3 - Stance Prediction
Before prediction started, tweet text is processed in preprocessing step. Preprocessing step is done by normalize text with remove stopwrods, remove emoji etc. After text is clear enough, text is converted to matrices with TF-IDF. The matrices is used to predict stance with machine learning algorithm.

## Step 4 - 

## Step 5

## Analysis
