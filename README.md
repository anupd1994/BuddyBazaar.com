# BuddyBazaar.com
A Trust based recommendation engine.
## Introduction
Most commercial recommender systems are strongly supported by the demographic information of users. Since some of the similarities within a network are caused by the influence and interactions of its members, it would be reasonable and feasible to develop a social recommendation based on the connections of individual users. In reality, people tend to be affected by the opinions of and suggestions by people with similar interests, shopping experts, and close friends. However, most of current social networking platform, such as Facebook and twitter, and electronic commerce platform, such as Amazon and Yahoo! Shopping, are independently operated. The supporting recommender systems are also independently deployed on the two kinds of platforms based on social factors and purchase history respectively. As a result, the electronic commerce (retailing) platforms generally do not consider social factors such as relationships and trust etc. among the users and the power of social influence is not exploited. Contrarily, social networking platforms generally do not consider online shopping related factors such as purchase history and product rating etc.So we've integrated a social network (in our case Facebook) and an online shopping site, wherein the user could ask for recommendations from his friends.
## Software Components
1. [mongoDB](https://www.mongodb.com/): [mongoDB](https://www.mongodb.com/)  is a free and open-source cross-platform document-oriented database.MongoDB is developed by MongoDB Inc. and is free and open-source, published under a combination of the GNU Affero General Public License and the Apache License.
2. [Oracle 10G](http://www.oracle.com/technetwork/database/database10g/overview/ds-general-oracle-database10gr2-se--132024.pdf): [Oracle 10G](http://www.oracle.com/technetwork/database/database10g/overview/ds-general-oracle-database10gr2-se--132024.pdf) is a object-relational database management system.
3. [Mahout](http://mahout.apache.org/) :[Mahout](http://mahout.apache.org/)  is a project of the Apache Software Foundation to produce free implementations of distributed or otherwise scalable machine learning algorithms focused primarily in the areas of collaborative filtering, clustering and classification.

## Data-sets
[MovieLens Dataset](http://grouplens.org/datasets/movielens/) is used in this project.

## HOW TO START
1. Create a new facebook app by visiting [here](devolpers.facebook.com). On creating an app you would get appID and app secret which is to be copied in the mentioned space in facebook.jsp. Please note to add localhost as domain name in settings tab of facebook app.
2. Download mongoDB from [here](https://www.mongodb.com/dr/fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.2.6-signed.msi/download). On downloading run mongod.exe as administrator and keep it running in the background. This act as mongodb server. Open mongo.exe and type "use movieLens". This creates a database movieLens. Now use mongoimport to import csv file to mongodb database. The csv file can be obtained from [here](http://files.grouplens.org/datasets/movielens/ml-100k.zip).
3. Download and install mongodb plugin for netbeans by following steps [given here](https://github.com/le-yams/nbmongo).
4. You are now ready to run the app.
