# anon-emoji

A partial replication of [The Shadowy Lives
of Emojis: An Analysis of a Hacktivist Collective’s Use of
Emojis on Twitter](https://arxiv.org/pdf/2105.03168.pdf). 

## Introduction
Anonymous is a prominent international hacktivist collective that often targets corporations and governments for politically motivated reasons. They are unusual for having a robust social media presence since they are involved in serious cybercrime. Do Anonymous-affiliated Twitter users’ emoji use differ from a typical user’s emoji use? How can we explain differences? What different meanings may different emojis have?

## Files listed in order of creation
* `main_collect.ipynb` - This notebook contains data collection and data filtering.
* `fwg.json, fwr.json` - These files contain the ids of followers and friends pulled from the seed accounts.
* `anonfwg.json`, `anonfwr.json` - These files contain the ids of Anonymous-affiliated candidates after checking for alphanumeric variations of 'anonymous' and 'legion'.
* `anonacc.json` - This file contains the ids, names, screen names, descriptions, and profile links of users from anonfwg.json and anonfwr.json with features to be used for supervised classification added.
* `affiliation.csv` - This file contains the manually labelled affiliations of users in anonacc.json.
* `atweets.json`, `rtweets.json` - These files contain Anonymous-affliated tweets and randomly sampled tweets.
* `main_analyze.ipynb` - This notebook contains data analysis and data visualization.
* `wc_anon_emojis.png`, `wc_random_emojis.png` - These files are WordClouds made with the [Twitter Color Emoji font](https://github.com/eosrei/twemoji-color-font) that display Anonymous-affliated tweet emojis and randomly sampled tweet emojis.