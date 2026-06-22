# AURA_players-analysis
Analysis of AURA players telemetry data using Python to clean and classify behaviour. The analysis is based on the code and documentation from [this Kaggle post](https://www.kaggle.com/code/pasindugeevinda/full-aura-pipeline), with some original modifications and upgrades. 

The telemetry data includes actions such as running, fighting and collecting items. We clean, transform and visualize the data to then:

1. Extract player performance features and detect outliers using PCA (my original contribution).

2. Feed it into an AI model to classify players among pre-defined archetypes (Explorer, Fighter, and Collector).

My main fix and contribution in 2. is identifying unreliable data in which the timeInCombat exceeded the duration time of the time intervals recorded, and adding a clarifying plot of the player gameplay over time. The removal of the bad data helped to improve the model accuracy. 

