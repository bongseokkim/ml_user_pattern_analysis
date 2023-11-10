# Competition : D CUP Google Analytics

## Introduction
- Predict future user behavior patterns using past DACON data.
- Awarded 2nd place in the private leaderboard.

## Description
- To reflect characteristics over time, date-related variables were added and LSTM was utilized.
- Through EDA, it was observed that values generally decrease on holidays, which led to assigning weights to holidays during LSTM modeling.
- A clear distinction was noted between weekdays and holidays within the same month. It was also found that weekdays in the same month show similar patterns, as do the holidays. To reflect these stable patterns, days were divided into holidays and weekdays, and further segmented according to the number of contests for more accurate predictions.
- Additional data analysis was conducted to identify features of days without regular patterns. This analysis helped in determining the number of logins and submissions from additional data, and separate features such as the actual number of logins and the total number of logins were developed.
- Various analyses and modeling processes suggested that the results should show extreme patterns. To achieve a more flexible outcome, the results of xgb and lstm, which have more moderate results, and the extreme patterns of extra were combined through Weighted Average Ensemble to derive the final results.

## Winner's Code Share
Visit the following link for the winner's code share:
[https://dacon.io/competitions/official/235683/codeshare/2340?page=1&dtype=recent&ptype=%20](https://dacon.io/competitions/official/235683/codeshare/2340?page=1&dtype=recent&ptype=%20)
