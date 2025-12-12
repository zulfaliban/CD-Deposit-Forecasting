# Forecasting U.S. CD Deposits — 1995–2025 (FRED WSMTMNS)

This project forecasts U.S. small-denomination time deposits using multiple time-series and machine-learning models.
Data is pulled directly from FRED using the fredr API.

Models Implemented

	•	ETS
	
	•	ARIMA
	
	•	ARIMAX (Fed Funds Rate as x-reg)
	
	•	XGBoost
	
	•	Multilayer Perceptron (MLP Neural Network)
	
	•	Ensemble (weighted combination)

Methods & Features

	•	Guerrero Box-Cox transformation
	
	•	KPSS stationarity testing
	
	•	Rolling averages & lag features
	
	•	Calendar variables (year, month)
	
	•	Harmonic seasonality terms
	
	•	Train/test split with forecasting horizon 2022–2025
	
	•	Volatility modeling (GARCH)

Files

	•	Forecasting-U.S.-CD-Deposits.qmd — full analysis and code
	
	•	Forecasting-U.S.-CD-Deposits.pdf — final written report
	
	•	95%_ARIMAX_interval.png — example forecast visualization
	
	•	references.bib — citation file

Key Insight

The 2022–2023 surge in CD deposits represents a structural break driven by rapid Federal Reserve rate hikes.
Because this regime does not exist in the training data, models cannot replicate the explosive shape of the test period — a theoretically correct outcome.
