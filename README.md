# Nintendo-Game-Ratings

The entirety of this repository concerns a Metacritic-sourced Nintendo games dataset (found [here](https://github.com/yaylinda/nintendo-games-ratings)), with per-title information on: platform, release date, user critic score, ESRB rating, developer(s), and genre(s). Part one covers exploratory data analysis of the user and critic score deltas at length, culminating in a Tableau dashboard with all interesting findings. Part two pivots to using the remaining dataset features in weighted association rule mining, with an end goal of quantifying what combinations of genres, developers, and ratings more consistently lead to higher scores (more to be added on this later).

### Review Score Delta Analysis

For a faster overview of my findings, peek inside the 'dashboard image.png' file; it even has some fancy color coordination going on. The delta in this was calculated by subtracting a scaled up version of the user score from critic score. Critic scores are typically out of 100, while users out of 10, leading to Delta = Critic - (User * 10). Overall, the averaged delta between the two sets of review scores was pretty small, -1.3%, with the median delta at -1.0, range of (-35.0, 37.0), and standard deviation of 8.9.
Fleshed out to a year by year basis, critic review scores were generally higher than user scores in the time outside 2002 - 2015. 2008 stands as the year with the largest user-biased delta (averaged user score greater than averaged critic score), and 2019 the largest critic-biased (vice versa to user-biased). By platform, the user-critic split is as follows: 3DS, DS, GBA, GC, Wii, and Wii U for user-biased, and iOS, N64, and Switch for critic-biased.

### Association Rule Mining

Loading...
