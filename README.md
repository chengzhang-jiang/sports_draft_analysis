# Sports Draft Analysis

According to Wikipedia, the NBA draft happens every year in June. It is where teams in the National Basketball Association (NBA) choose players who have never played in the NBA before. This analysis is intended to shed some light on which college stats are most predictive in terms of their early success. The teams can take advantage of it as a reference when scouting players. This can also help recognize talents that deserve the attention and ‘draft busts’ who are overestimated. 

I applied several machine learning models in order to predict players performance early in their professional career. Among regularized linear models, KNN and random forests, random forests stand out as the best with lowest mean square error (MSE) in test data, 1.536. Three-year VORP is used as a proxy of ‘early success’, which is specifically NBA prospects’ value above replacement over their first three seasons in the league. I take into account college stats including games they played and per-game measures like field goals, field goals attempted, free throws, assists, rebounds, steals, blocks and turnovers. Since international players are in face of different levels of competition compared to American players, the analysis does not include international players. In training the model, college prospect modeled are drafted between 2011 through 2017.

The NBA and college data comes from four sources: Basketball Reference, Sports Reference, NBA.com, and Draft Express. The data tables listed above are collected with **web scraping** as a part of the codes provided in this repository.

Regarding the findings, the most predictive variables for early NBA success (in terms of VORP) are steals, defensive rebounds, games, two-point field goal attempts and height. The least predictive variables in the model are the player’s wingspan, turnovers, assists, blocks and personal fouls. The top 3 and bottom 3 variables are shown above in graph 1 with their importance scores output by the algorithm. In 2018 draft projection, the most promising player identified by the model is Mohamed Bamba with a ranking of 6 in the real draft. Trae young, as a rising star regarded by many fans, ranks the second in my projection with a projected VORP being 5. Interestingly, Alize Johnson ends up being in the top tier but his real order in the draft is 50, indicating he could be a player with high potential but is not fairly valued. The last player is Grayson Allen whose ranking in 2018 draft is 21, meaning the player is overrated to some extent.

Reference:
- https://www.cmusportsanalytics.com/2017-nba-draft-forecast/
- http://www.basketball-reference.com/
- http://www.draftexpress.com/
- http://www.sports-reference.com/
- https://www.nba.com/
