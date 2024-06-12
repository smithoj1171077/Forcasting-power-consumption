# Forcasting-power-consumption

# background
While global warming has been widely recognised as a pressing issue, organisations and governments still need to overcome the economic and technical hurdles transitioning away from carbon emitting energy sources. The sucess of this transition to renewable energies sources hinges on their ability to consistently meet the demands of the energy grid. Despite the increasing sophistication of renewable technologies there are two concerns which hinder enuthsiastic adoption at the rate necessary to meet the emissions targets layed out in the Paris Agreement. Namely, wind and solar generation capacities are in significant respects, dependent on stochastic weather events out of human control, and that demand for power flucuates greatly, renewable power sources are less straight forward to scale up and down than carbon based power. The focus of this project is on the second argument, I will explore these power demand patterns and experiment with two different modelling approaches to forcasting them, this will provide insights into how we can plan renewable energy grids to reliably meet the demands of Australian households. 

# Dataset
The dataset is derived from the OpenNem dashboard, an initiative by The University of Melbourne Climate & Energy College. It provides a highly granular time series of power consumption and generation for across different energy sources in Australia. 
https://opennem.org.au/energy/nem/?range=30d&interval=1d&view=discrete-time

# Experiments
The experiments will revolve around predicting the power consumed in Australia, of particular interest is see how effectively different modelling techniques can pick up on cyclical patterns such as the day-night cycle, weekly variations such as weekends vs weekdays, and 
seasonal variations such as summer vs winter. There are two models I have chosen to evalute, a traditional autoregressive time series model SARIMA which is designed to capture seasonal patterns, and a recurrent neural network variant called an LSTM. 

