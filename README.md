# anon-emoji

This is a partial replication of [this study](https://arxiv.org/pdf/2105.03168.pdf). 

Anonymous is a prominent international hacktivist collective that breaks into computer systems for politically motivated reasons. They have a very extensive history of cyberattacks beginning around 2003. Anonymous also has a robust social media presence. It is unusual for a hacking group to be so open when they are involved in serious cybercrime against governments. I am interested in analyzing their public image. 

Emojis has become common in digital communication for efficiently and effectively conveying emotions. They have many associated meanings that can be implied. Emojis are especially well-suited for elevating self-expression on social media. 

I am curious about how hacktivists appear on social media. Since I am very supportive of emojis and I am interested in what Anonymous chooses to share, I will be looking at how Anonymous-affiliated Twitter users’ emoji use differs from a typical user’s emoji use. How can we explain differences? What different meanings may different emojis have? 

* main_collect.ipynb - This notebook contains data collection and data filtering.
* fwg.json, fwr.json - These files contain the ids of followers and friends pulled from the seed accounts.
* anonfwg.json, anonfwr.json - These files contain the ids of Anonymous-affiliated candidates after checking for alphanumeric variations of 'anonymous' and 'legion'.
* anonacc.json - This file contains the ids, names, screen names, descriptions, and profile links of users from anonfwg.json and anonfwr.json with features to be used for supervised classification added.
* affiliation.csv - This file contains the manually labelled affiliations of users in anonacc.json.
* atweets.json, rtweets.json - These files contain Anonymous-affliated tweets and randomly sampled tweets.
* main_analyze.ipynb - This notebook contains data analysis and data visualization.
* wc_anon_emojis.png, wc_random_emojis.png - These files are WordClouds using Anonymous-affliated tweet emojis and randomly sampled tweet emojis.
