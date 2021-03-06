---
layout: post
title: Best mates in the Premier League
description: >
  Who's played the most minutes with who?
author: author1
image: /assets/img/2020-06-11-Best-Mates/skysports-ben-mee-james-tarkowski_4918858.jpg
noindex: true
categories: [football]
tags: [Football, Premier League, Analytics]
---

["The iconic starting XIs who rarely played together"](https://www.bbc.com/sport/football/51491041), written by BBC sport, was one of the more interesting retrospective football pieces I came across this year. While not exactly the inspiration for idea behind this post, the concept reminded me of this first little side project I did. A couple of summers ago, I thought about looking at the number of minutes played together between any pair of players. As a football fan I've definitely heard on numerous occasions commentators mentioning that "so-and-so are only starting together for the Xth time this season" and fans/pundits stressing the [value](https://www.footballwhispers.com/blog/5-centre-backs-liverpool-target/) [of](https://theprideoflondon.com/2020/06/08/chelsea-consistent-center-back-pair-can-make-difference/amp/) [having a](https://www.football365.com/news/man-utd-smalling-and-the-seven-year-partner-search) [consistent](https://www.skysports.com/football/news/11667/11477591/manchester-united-defensive-frailties-is-jose-mourinho-right-to-worry) [centre-back](https://theathletic.co.uk/1665272/2020/03/11/chelsea-centre-back-tomori-rudiger-christensen-zouma/) [partnership](https://www.sportskeeda.com/football/consistency-paying-dividends-premier-league-best-centre-back-combinations). While obviously we shouldn't expect such a simple measure to correlate well with actual team performance or chemistry, it could offer a little insight into why some teams aren't gelling so well. At worst, we get some fun titbits of information out of it!  

## Getting the Data

I used data from Transfermarkt.com for this project, which provides the following per game stats for each player for every season in their record:

- Number of minutes played
- Minute sub-ed in  
- Minute sub-ed out


Scraping the data was with much to credit to the tutorial by [FCPython](https://fcpython.com/blog/introduction-scraping-data-transfermarkt). A still rather messy version of this code is available [here](https://github.com/glad94/footy-scraper). Should also mention that FCrSTATS released a [Python package](https://github.com/FCrSTATS/tyrone_mings) for scraping Transfermarkt very recently as well. 

## Centre-Backs

I mentioned Centre-Backs at the beginning so let's look at who's been the best of mates so far this season. 


![PL 1920](/assets/img/2020-06-11-Best-Mates/CB_mins_1920.png)
I've taken the most shared minutes between any pair of players designated as a "Centre-Back" on Transfermarkt. Fernandinho is only exception..
{:.figure}

At the very top we have James Tarkowski and Ben Mee of Burnley FC whom you'd also notice have played every single minute of their season together so far! This perfectly consistent has certainly been a credit to their decent season so far, with the Claret sitting 10th place in both the overall league and [goals conceded](https://www.premierleague.com/stats/top/clubs/goals_conceded) table. The benefits of having a consistent centre-back pairing are certainly more appreciable for the next three teams: Leicester, Sheffield Utd and Man Utd; who have the 3rd, 2nd and 4th best defence respectively. On the flip side, we see that the most minutes played between Man City's "actual" centre-backs is only a measly 360 min. Even if you factor in Fernandino playing in that position for pretty much this whole season, his 985 min with Otamendi is still the 4th lowest in the league. It has been a disappointing season so far for the reigning champions and it's no surprise that their defensive injuries and resulting instability have been cast under the spotlight [on](https://www.theguardian.com/football/2020/jan/19/pep-guardiola-amyeric-laporte-manchester-city) [multiple](https://www.skysports.com/football/news/11679/11829745/manchester-citys-defensive-problems-could-cost-them-their-title) [occasions](https://www.forbes.com/sites/grahamruthven/2019/10/11/manchester-citys-defensive-woes-shouldnt-have-come-as-such-a-surprise/#d2351d411860). Like City, Norwich also haven't been helped by an inconsistent centre-back pairing due to chronic injuries, though the repercussions are certainly more dire with the Canaries staring down the barrel of relegation while possessing the 2nd worst defence (52 GA). The league's worst defence, Aston Villa (56 GA), may also be pondering what might've been if they got more consistent playing time between their defenders. 

As previously mentioned we should in no way expect this simple measure to correlate well with team performance as other factors e.g. quality of players/coaching; the other 9 active players; quality of squad/rotation players, are logically more important than how well any 2 players "know" each other on the pitch. The team that makes the most nonsense of this metric is no doubt the champions-in-waiting Liverpool, who have conceded the least goals (22) despite their centre-back partnership being one of the less consistent ones. Southampton, West Ham and Bournemouth,  who are in the top half of this table have the next worst defences in the league. 

All that being said, let's look how teams performed in this for the previous 2 seasons.

![alt-text-1](/assets/img/2020-06-11-Best-Mates/CB_mins_1819.png) 
![alt-text-2](/assets/img/2020-06-11-Best-Mates/CB_mins_1718.png)

Again we see Liverpool making a joke of this metric in 2018/19 with them also having the best defence last season. It's probably also testament to how solid a defender van Dijk is such that it doesn't really matter whether he has a consistent partner or not. With 81 goals conceded, Fulham really should've invested in more than just Le Marchand and Ream sharing 1113 min on the pitch. However, we also start to see more that a consistent defensive pairing can only take you that far, with Huddersfield, Cardiff, West Brom and Swansea all getting relegated over the last 2 seasons despite scoring high in this metric. Finally, just for fun, I decided to see what plotting goals conceded vs shared minutes would look like: 


<p align="center">
  <img src="/assets/img/2020-06-11-Best-Mates/Min_vs_GA.PNG">
</p>
Taking Data from the last 10 seasons from 2009/10 (excluding 2019/20)
{:.figure}

It's a bit of a mess, which is expected to be fair as at the end of the day, there's large discrepancies in player quality/budgets in a 20-team league for the measure to always reflect something sensible for every team. 

Now that we've looked at how the minutes have been shared amongst centre-backs, let's take a look on the other side of the pitch.

## Forwards

![PL FW 1920](/assets/img/2020-06-11-Best-Mates/FW_mins_1920.png)
Similarly here I've taken the most shared minutes between any pair of players designated as a "Forward" on Transfermarkt.
{:.figure}

Despite topping this table, Crystal Palace currently have the 3rd worst attacking record (26 goals scored), with Zaha chipping in only 3 goals so far compared to 10 and 9 in his past 2 seasons respectively. Having a settled front 2 (or 3 rather) is certainly paying dividends again for Liverpool, with Salah-Firmino-Mane also having scored 49 of Liverpool's 98 goals in all competitions in 2019/20. At the bottom we find Sheffield Utd who have exceeded expectations on the back of a solid defensive foundation, but struggled for goals with only 30 so far (15th). Newcastle likewise have been experiencing goal-scoring woes with only 25 to show for (joint last with Norwich). 

While I won't go into detail about shared forward minutes for the previous 2 seasons, I'll leave their equivalent figures below for your interest. One thing of note is that Liverpool and Crystal Palace have also been in the top 3 over these last 2 seasons. 

## Aside
There were some other things that I briefly explored from the data I gathered out of my own interest as Man Utd fan. 

## Rashford-Martial FC
Under Jose Mourinho's reign I was often frustrated at how Rashford and Martial were never really given a proper run in the team, let alone together. I must admit I have a real soft spot for these two, Martial for instantly making a mockery of that ["What a waste of money"](https://therepublikofmancunia.com/wp-content/uploads/2016/04/img_8812-940x759.jpeg) headline and Rashford for emerging from virtually out of nowhere to give us one of the [all-time best Arsenal Fan TV moments](https://www.youtube.com/watch?v=-LOioe5fXPo). While Van Gaal unleashed this pair without any leashes, I struggle to recall matches where these two started or played together...(Man City H and Brighton A 17/18 in my immediate memory at most), so I decided to look at what the numbers said.  

<p align="center">
  <img width="491" height="267" src="/assets/img/2020-06-11-Best-Mates/MaRash_mins.png">
</p>



While the two shared 705 minutes from just February onward in 2015/16, this number dropped to the 500s under Jose, who also started viewing the 2 as competitors for the LW spot in 2017/18 (until [you know who](https://www.youtube.com/watch?v=CCk30hIr1Sw) arrived in January). Thankfully for me, things have been on the up for these two since Solskjaer arrived who has fully put his trust in them to lead the line. With 35 goals between them already this season, Solskjaer's faith appears to be paying off and hopefully, this is merely the first sign of greater things to come.

## Unlucky Mourinho?
I also decided to look at how consistent Man Utd's centre-back pairings over the last 10 seasons.

![MUCB](/assets/img/2020-06-11-Best-Mates/MU_CB_mins.png)

While many fans never really warmed up to Mourinho's vision of a defensively-minded Man Utd, I personally also feel that he never quite took the defence to where he wanted them to be and more often than not, [David de Gea](https://www.goal.com/en-sg/news/de-gea-is-no-longer-masking-mourinhos-man-utd-problems/1xs6njhx02imh1t9birfqmochw) was the man holding the fort. Seeing how everpresent Maguire-Lindelof have been this season, I can't help but wonder slightly what could've been if Mourinho had got his man in [summer 2018](https://www.independent.co.uk/sport/football/premier-league/man-utd-transfer-news-jose-mourinho-ed-woodward-latest-a9219881.html?utm_source=reddit.com). 

## Closing Thoughts
While I don't think there was ultimately much analytical insight gained from this exercise, I did learn some interesting things along the way and I'm quite satisfied that I've managed to take this first little side project this far i.e. finally 'completing' something I started on 2 years ago. I guess at the end of the day, having consistent player pairings can help to a certain extent as seen from the several examples above. Beyond shared player minutes, there are certainly better and more sophisticated metrics out there that attempt/can capture player or team chemistry. One [paper](http://www.sloansportsconference.com/wp-content/uploads/2020/02/Bransen_paper_player_chemistry.pdf) I came across recently quantified the chemistry between player pairs by taking also into account their on-pitch actions via the [VAEP framework](https://dtai.cs.kuleuven.be/sports/vaep?toggle=explore). So, definitely something for me to dive into further and perhaps continue exploring in the future!  
