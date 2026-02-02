# IPL Win Probability Predictor

A machine learning project to predict the probability of winning for Indian Premier League (IPL) cricket matches using historical match and delivery data.

## Project Overview

This project analyzes IPL cricket data and builds predictive models to estimate the likelihood of a team winning a match. It uses historical match statistics, team performance metrics, and game delivery data to make predictions.

## Project Structure

```
IPL_win_probability/
├── app.py                          # frontend
├── requirements.txt                # Python dependencies
├── README.md                       # readme
├── data/                           # data
│   ├── matches.csv                # IPL match information
│   ├── deliveries.csv             # Ball-by-ball delivery data
│   ├── teams.csv                  # Team information
│   ├── teamwise_home_and_away.csv # Home/away statistics
│   └── most_runs_average_strikerate.csv  # Player statistics
├── notebooks/                      
│   └── model.ipynb                # Model development notebook
└── models/                         # Trained model storage
```

## Data Description

- **matches.csv**: Contains match-level information including:
  - Match ID, Season, Date, Venue, Teams, Winner, etc.

- **deliveries.csv**: Contains ball-by-ball delivery data including:
  - Match ID, Inning, Teams, Batsman, Bowler, Runs, Dismissals, etc.

- **teams.csv**: Team information and metadata

- **teamwise_home_and_away.csv**: Historical home and away performance metrics

- **most_runs_average_strikerate.csv**: Player batting statistics

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Kushagra3355/IPL_win_probability.git
   cd IPL_win_probability
   ```

2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Required Dependencies

The project uses the following main libraries:

- pandas: Data manipulation and analysis
- numpy: Numerical computations
- scikit-learn: Machine learning models
- jupyter: Interactive notebooks

## Usage

### Running the Application

```bash
python app.py
```

### Developing Models

Open the Jupyter notebook for interactive model development:

```bash
jupyter notebook notebooks/model.ipynb
```

## Model Development

The `notebooks/model.ipynb` contains:

- Data loading and exploration
- Feature engineering from match and delivery data
- Model training and evaluation
- Win probability predictions

## Features Used

- Team performance metrics (wins, losses)
- Home/away advantages
- Player statistics (runs, strike rates)
- Venue information
- Historical head-to-head records

## Model Output

The trained models predict the probability of a team winning a match, which can be used for:

- Match outcome analysis
- Risk assessment
- Betting insights
- Performance analytics

## Future Enhancements

- Real-time prediction during live matches
- Integration with live match APIs
- Enhanced feature engineering
- Ensemble model approaches
- Web interface for predictions

## Author

Kushagra3355

## License

This project is open source and available under the MIT License.
