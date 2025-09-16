# DA_Project

- The team that has won the **most tosses** is shown by `matches_df['toss_winner'].value_counts()`.[1]
- After winning the toss, the most common decision is displayed by `matches_df['toss_decision'].value_counts()`. The bar chart shows whether **batting** or **fielding** is the preferred choice.[1]
- The number of times the **chasing team has won** the match is displayed by `chasing_team_wins`, which is the count of matches where toss and match winner are the same.[1]
- The team that has **played the most matches** is the one with the highest sum from `matches_df['team1'].value_counts() + matches_df['team2'].value_counts()`.[1]
- The team with the **most match wins** is shown by `matches_df['winner'].value_counts().idxmax()`.[1]
- The batsman with the **most balls faced** is found via `balls_df.groupby('batsman')['ball'].max().idxmax()`.[1]
- The **leading run-scorer of all time** is obtained from `balls_df.groupby('batsman')['batsman_runs'].sum().idxmax()`.[1]
- The **top wicket-taker** is listed by `balls_df.groupby('bowler')['player_dismissed'].count().sort_values(ascending=False)`.[1]
- The player with the **most Man of the Match awards** is given by `matches_df['player_of_match'].value_counts().idxmax()`.[1]

### Key IPL Analytics Results

#### Toss and Winning Patterns
- The team with the **most toss wins** can be identified in the first output of `toss`.[1]
- The most common toss decision is **fielding** (electing to bowl).[1]
- Winning the toss does not guarantee a match win; this relationship is quantified by `toss.value_counts()`.[1]

#### Team Performance
- Most matches played: Refer to `most_matches_counts.idxmax()` for the top team.[1]
- Most matches won: `matches_df['winner'].value_counts().idxmax()` gives the leading team.[1]
- Highest winning percentage: Also aligns with most wins, as per the previous code output.[1]

#### Individual Records
- Most balls faced: Output from `most_balls.idxmax()`.[1]
- Leading run-scorer: Found via `leading_run_scorers.idxmax()`.[1]
- Most fours: Top player returned by `most_fours.idxmax()`.[1]
- Most sixes: Top player from `most_six.idxmax()`.[1]
- Leading wicket-taker: Highest value in the `wicket_counts` output.[1]
- Most Man of the Match awards: See result of `most_mom.idxmax()`.[1]

#### Stadiums and Venues
- Stadium hosting the most matches: The venue from `matches_df['venue'].value_counts().idxmax()`.[1]

#### Season-Wise Statistics
- Counts for fours, sixes, and total runs from boundaries per season are found via the respective grouped `.count()` and `.sum()` outputs and visualized in bar charts.[1]

All results presented above are calculated and summarized directly from the IPL mini-project Python analysis script.[1]

[1](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/97486039/d34da377-6570-4356-8b87-97643599a5bd/ipl_mini_project.py)
