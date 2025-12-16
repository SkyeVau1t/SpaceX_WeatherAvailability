# SpaceX_WeatherAvailability
ATMS 523 end of semester project
1. Predicting SpaceX Launch Weather Outcomes Using Machine Learning
2. The objective of this project is to develop a machine learning model that predicts the likelihood of a SpaceX launch proceeding or being scrubbed due to weather conditions. The model will be trained on historical SpaceX launch data paired with corresponding weather observations and forecasts to reverse-engineer the company’s weather-related launch criteria, often referred to as “weather launch commit criteria” or placards. The final tool will allow a user to input an upcoming launch window and receive a probabilistic confidence of whether the launch is likely to proceed given forecasted conditions.

3. The primary datasets will include:

SpaceX launch history data (from public APIs such as SpaceX APILinks to an external site.) detailing launch dates, times, outcomes, and scrub reasons.

Historical weather data from ERA5 reanalysis, covering weather variables such as surface wind speed, cloud base height, precipitation, lightning activity (KSC Field Mills), and temperature for Cape Canaveral and the Kennedy Space Center region.

The analysis will focus on launches from 2010–2024, covering roughly 300–400 launches and corresponding weather conditions. Temporal resolution will be hourly, and spatial coverage will center on the Cape Canaveral launch complex (28.5°N, 80.6°W).

4. I expect to find a strong correlation between specific weather variables, particularly wind speed, cloud coverage, and lightning risk, and launch outcomes. The resulting machine learning model (likely a logistic regression or random forest classifier) should be able to predict launch or scrub outcomes with moderate to high accuracy, potentially reconstructing SpaceX’s implicit weather decision thresholds. The end product will be a Jupyter Notebook workflow capable of generating a percent confidence of launch for upcoming missions based on forecast data, demonstrating how data-driven methods can approximate operational decision-making in aerospace meteorology. I also expect to have to separate each iteration of Falcon design in the learning process, since placards can change based on engine improvement or landing gear updates. 
