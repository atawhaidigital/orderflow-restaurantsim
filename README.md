# Order Flow - Restaurant Profitability Simulation Engine

Order Flow is a restaurant profitability simulation engine created using Plumber API, designed for probabilistic modelling and scenario analysis with a strict focus on data integrity.
The tool helps to identify the most profitable delivery channels, forecast app performance, and provides actionable insights. 

The project aims to help restaurants visualise and understand the growth of delivery apps and how they will perform for their restaurant business, enabling them to make data-driven marketing decisions.

# What problem Order Flow solves?
Food delivery platforms are growing rapidly, but many restaurants struggle to understand:
	Which delivery apps are actually profitable after fees and commissions?
	How do changes in order mix affect overall margins?
	Does increased volume translate to real profit?
	How do future growth scenarios impact their business?

# What does the simulator do?
At a high level, Order Flow allows restaurants to:
	Model multiple delivery channels and order flows
	Simulate changes in volume, fees, and customer behaviour
	Compare profitability across apps and scenarios
	Understand how channel mix affects total revenue and margin

# Data integrity as a design principle
While profitability is the primary goal, Order Flow is intentionally strict about analytical correctness:
	Shares represent composition and must sum to 100%
	Rates represent likelihood and are treated separately
	Inputs are validated to prevent ambiguous or misleading assumptions

# Use cases
	Evaluating delivery app performance for a restaurant
	Forecasting the impact of marketing spend on order mix
	Testing growth scenarios before committing the budget
	Supporting data-driven pricing and promotion decisions

# Project status
The project is under active development and currently focuses on:
	Core simulation logic
	Profitability modelling
	API stability and clarity

# Who should use this simulation
	Restaurant owners exploring delivery strategies
	Marketing managers deciding where to allocate spend
	Analysts evaluating delivery app performance and growth scenarios 

# How to Use the Simulator

# Set up your scenario
	Decide which delivery apps you want to include (UberEats, Deliveroo, etc.)
	Enter the total monthly orders across all delivery channels (in-store, delivery apps, expected self-delivery orders if you are running self-delivery)

Assign a percentage of total orders to each channel. Percentages must sum to 100%.
  # For example: 
    Total monthly orders = 1,000
    UberEats = 50% → 500 orders
    Deliveroo = 30% → 300 orders
    DoorDash = 20% → 200 orders  

  # Formula:
  Channel = (Orders for that channel/total monthly orders) x 100

  UberEats = (500/1000) x 100 = 50%

  Check: 50% + 30% + 20% = 100% ✅

This ensures the simulator distributes orders correctly and calculates channel profitability accurately

# Run the simulation
	The simulator calculates profit per channel, factoring in commission fees and other assumptions 
	It also forecasts app performance over time.
	
# Interpret the results
	Compare delivery channels by profitability.
	Identify opportunities to adjust marketing or channel mix.
	Make informed business decisions based on simulated scenarios.

# Key Insights
	Channels are compared fairly using realistic assumptions.
	Shares and percentages are internally validated to reflect true proportions.
	The simulator highlights how growth in one channel affects total profitability.

