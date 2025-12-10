# 🏀 CBB xP Analytics

**Interactive College Basketball Shot Charts with Expected Points Analysis**

Created by [@pickleo7](https://twitter.com/pickleo7) | Picklelytics

---

## 📊 What is xP?

**Expected Points (xP)** is a metric that calculates the probability a shot will be made based on:
- Shot distance from the basket
- Shot angle
- Shot type (rim, mid-range, three-pointer)

Our model is trained on thousands of NCAA shot attempts to predict the expected point value of each shot.

## 🎯 Features

- **Interactive Shot Charts**: Hover over any shot to see detailed stats
- **Player-by-Player Analysis**: See which players over/underperformed
- **Court Visualization**: Accurate NCAA court dimensions and shot locations
- **Expected vs Actual**: Compare what the model expected vs what actually happened

## 🔗 View Games

Visit the [interactive dashboard](https://pickleo7.github.io/cbb-xp/) to explore games.

### Recent Games

- [Alabama 97, UTSA 55 - Dec 7, 2025](games/20251207_UTSA_vs_Alabama_210210/shot_chart.html)

*More games added regularly!*

## 📈 Methodology

Our xP model uses:
- **LightGBM Classifier** trained on NCAA shot data
- Features: shot distance, angle, normalized coordinates
- **Hierarchical Estimation**: Player-specific (25+ shots) → Team-specific (100+ shots) → League average
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
Data provided by CollegeBasketballData.com

---

*Last Updated: December 10, 2025*
