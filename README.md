# 🏀 CBB xP Analytics

**Interactive College Basketball Shot Charts with Expected Points Analysis**

Created by [@pickleo7](https://twitter.com/pickleo7) | Picklelytics

---

## 📊 What is xP?

**Expected Points (xP)** is a metric that calculates the probability a shot will be made based on:
- Shot distance from the basket
- Shot angle
- Shot type (rim, mid-range, three-pointer)

The model is trained on millions of NCAA shot attempts to predict the expected point value of each shot. Think of this as the following: If the average D1 basketball player took a shot from this location on the floor, what is the probability of a make multiplied by the value of the shot area? (60% probability of making a layup from 5 feet away = 1.2 Expected Points)

The focus of the model's research is not to focus on an individual shot's expected value in the same way that this can be used to show the low likelihood of a long range shot in soccer. While this will of course be fun to see when we get the first 3/4 Court heave in a Do or Die situation in March, the real benefit is lining up hundreds and thousands of shots by players and teams to see what's going on under the hood. We will use the macro trends shown by the data to showcase player skill, efficient offenses, stringent defenses, underlying momentumn throughout a season, and showcase coaches and systems that do the best job at creating ideal opportunities for their players.

Consider this the first step of my research in granular analysis of the wonderful sport of college basketball. 

## 🎯 Features

- **Interactive Shot Charts**: Hover over any shot to see detailed stats
- **Player-by-Player Analysis**: See which players over/underperformed
- **Expected vs Actual**: Compare what the model expected vs what actually happened. We break this down by type of shot (2PT/3PT/FT) to compare scoring to expected efficiency.
- **Who Deserved to Win?** 10,000 Monte Carlo simulations on the model outcomes of each shot with coordinate data from the game to analyze which team created the best chances for themselves, and limited their opponents' chances.

## 🔗 View Games

Visit the [interactive dashboard](https://pickleo7.github.io/cbb-xp/) to explore games.

Game breakdowns will showcase xP totals by category, simulations of outcomes based on the shots taken, interactive shot charts, and player based analysis. 

The site will be updated as soon as game data is available. Users can "Follow" teams, select games by date, team, or league. 

*More games added regularly!*

## 📈 Methodology

Our xP model uses:
- **LightGBM Classifier** trained on NCAA shot data
- Features: shot distance, angle, normalized coordinates for standard analysis
- **Hierarchical Estimation**: Player-specific (25+ shots) → Team-specific (100+ shots) → League average. Not all games have complete shot coverage. But, we can estimate the types of shots a player or team takes and assign an xP value to a shot for which we do not have coordinates.
- Data from [CollegeBasketballData API](https://collegefootballdata.com)

## 🛠️ Tech Stack

- **Data**: CollegeBasketballData API
- **Model**: Python, LightGBM, scikit-learn
- **Visualization**: Plotly (interactive charts)
- **Graphics**: Matplotlib (Twitter graphics)
- **Hosting**: GitHub Pages

## 📱 Follow Along

- Twitter: [@pickleo7](https://twitter.com/pickleo7)
- Check back for new games and analysis!

## 📝 License

Charts and analysis by @pickleo7 | Picklelytics
Data sourced from CollegeBasketballData.com

---

*Last Updated: December 10, 2025*
