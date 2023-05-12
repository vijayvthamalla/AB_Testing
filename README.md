# AB_Testing
we will analyze the result of an A/B test where the first gate in Cookie Cats was moved from level 30 to level 40. In particular, we will analyze the impact on player retention and game rounds

Cookie Cats is a popular mobile game that aims to engage and retain players. In this analysis, we examine the results of an A/B test conducted on two versions of the game, gate_30 and gate_40, to determine the impact on player engagement and retention. The goal is to identify which version leads to higher player retention and game rounds played.

The dataset used for the analysis contains information on user IDs, game versions, the number of game rounds played (sum_gamerounds), and player retention at 1 day (retention_1) and 7 days (retention_7) after installing the game. The dataset consists of 90,189 observations.

We begin by loading the data and performing exploratory data analysis. The dataset includes one object variable (version), two integer variables (userid and sum_gamerounds), and two boolean variables (retention_1 and retention_7). There are no missing values in the dataset.

To ensure accurate analysis, extreme outliers in the sum_gamerounds variable are removed. Summary statistics are then recalculated, showing a count of 90,188 observations, a mean of 51.32 game rounds played, and a maximum of 2,961 game rounds.

We compare the two game versions (gate_30 and gate_40) based on the sum_gamerounds variable. Both versions have similar summary statistics, with a median of 16 game rounds and a mean of around 51 game rounds. However, statistical significance between the two groups is yet to be determined.

We investigate player retention by analyzing the retention_1 and retention_7 variables. Approximately 55% of players did not return to play the game after 1 day of installation, and 81% did not return after 7 days. We further explore the relationship between game versions and retention, finding similarities in summary statistics but without statistical significance.

We combine the retention_1 and retention_7 variables to create a new variable, "Retention," which indicates whether a player remained active after both time points. Both game versions show similar results, with around 12,000 players (14% of the total) exhibiting continued engagement with the game.

**Conclusion:**
The analysis of the A/B test for the Cookie Cats mobile game reveals no significant differences between the gate_30 and gate_40 versions regarding player engagement and retention. Both versions show similar patterns in terms of game rounds played and player retention, suggesting that neither version has a clear advantage over the other.

It is important to note that this analysis only considers the variables provided in the dataset. Further exploration and analysis of additional factors, such as user demographics, in-app purchases, or gameplay features, may provide deeper insights into player engagement and retention.

Based on these findings, the decision to implement either version should consider factors beyond player engagement and retention, such as development and maintenance costs, user feedback, and other business objectives.

Overall, this analysis highlights the importance of rigorous statistical testing and comprehensive data analysis in A/B testing to inform decision-making and improve the effectiveness of mobile game development and optimization strategies.
