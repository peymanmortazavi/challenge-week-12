# Challenge Week 12 Submission Template

Peyman Mortazavi

# Reddit Data Challenges

## Challenge 1

![Image](ch1.png)

## Challenge 2

It's interesting that our data has some issues, I wanted to find the ratio <number of posts with no like>/<number of posts> but we only have 'null' for likes.

db.reddit.distinct("likes") returns [ null ]

## Challenge 3

You could find interesting social facts. Like finding top downvoted posts, that's what people in society--or at least in reddit don't like.

## Challenge 4

What majority of topics are about/likes and dislikes in the community. Like you could see if majoriy of people in reddit are tilted towards a political party or not.


## Challenge 5

[Link to Code or pasted code]
[Answer]

## Challenge 6

It'll affect our analyze dramatically. The people who are good writers in reddit space and often attract many upvotes will remove many raddits from our data.

## Challenge 7

Yes, very much. If we only study posts or people whose post are upvoted often, our results and conclusion will be biased.

## Challenge 8

We'll be biased towards popularity.

## Challenge 9

Private subraddits are filtered out.
Only popular raddits are included.

## Challenge 10

To analyze real data modified data and see if the result is biased toward a specific direction.


# Yelp and Weather 

## Challenge 1

db.precipitation.aggregate([{"$match":{"date":{$regex:/20100425/}, "station.name":"MADISON DANE CO REGIONAL AIRPORT WI US"}},{"$group":{"_id":null,"total":{"$sum":"$hpcp"}}}])

ANSWER: 62

## Challenge 2

[Query snippet]

db.normal.aggregate([ {$match: {"DATE": {$regex: /20100425/}, "STATION_NAME": {$regex: /LAS VEGAS/}}}, {$group: {"_id":null, avg: { $avg:"$HLY-WIND-AVGSPD"}}} ])

ANSWER: 110.08333333333333

## Challenge 3

db.businesses.count( { city: "Madison", state: "WI" } )

ANSWER: 1630


## Challenge 4

db.businesses.count( { city: "Las Vegas", state: "NV" } )

ANSWER: 12021

## Challenge 5

db.businesses.count( { city: "Phoenix", state: "AZ" } )

ANSWER: 7499

## Challenge 6 [BONUS]

[Code]
[Answer]



