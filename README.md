# Revenue_Forecasting_Performing_Arts_Setting
Forecastability analysis and ticket sales forecasting using booking curve data and information-theoretic diagnostics.
This repository contains work on ticket sales forecastability and forecasting for performing arts events.
## Business Problem

Performing arts organisations rely on ticket sales forecasts to plan marketing activity, manage pricing strategies, and monitor revenue risk across productions.

However, ticket sales typically follow a **booking curve**, where demand evolves over time as the performance date approaches.  
Forecasting too early can be unreliable if the early booking data contains limited predictive signal.

This project investigates how predictable ticket sales are during the booking window and develops forecasting methods tailored to performing arts ticketing data.

## Project Objective

The goal of the project is to:

- evaluate the **forecastability of ticket sales booking curves**
- identify how much early sales behaviour predicts later demand
- determine whether **different tiers of productions exhibit different forecastability patterns**
- develop forecasting workflows informed by booking curve dynamics

## What Was Achieved

The project produced two main analytical components:

**1. Forecastability Assessment**

Using **Auto Mutual Information (AMI)**, the project evaluates how information about future ticket sales decays across the booking window.  
This analysis helps estimate the **forecastability horizon** of theatre booking curves.

**2. Ticket Sales Forecasting**

A forecasting workflow was implemented using features derived from ticketing data, including:

- Tier classification
- Order Days from Opening
- Days within the season
- Venue capacity and event characteristics

The AMI analysis informs feature design and helps identify where reliable forecasting is possible within the booking cycle.

## Key Contribution

The project demonstrates how **information-theoretic diagnostics can support practical forecasting in a performing arts setting**, linking booking curve structure with predictive modelling decisions.

## Contents

- `notebooks/01_AMI_Assessment.ipynb`  
  AMI-based assessment of booking-curve forecastability by tier.

- `notebooks/02_Ticket_Sales_Forecast.ipynb`  
  Forecasting workflow for ticket sales using features such as Tier, Order Days from Opening, and Days in Season.

## Key Variables

- **Order Days from Opening** – booking curve time index
- **Ticket Count** – tickets sold
- **Event** – production identifier
- **Tier** – demand tier classification
- **Days in season** – position within the performance run
- **Venue_Capacity** – theatre capacity
- **Season order** – season sequencing variable
- **SeasonMaxDay** – maximum observed booking day for the event
- 
## Project Structure

Revenue_Forecasting_Performing_Arts_Setting

├── notebooks  
│   ├── 01_AMI_Assessment.ipynb  
│   Forecastability analysis using Auto Mutual Information (AMI)  
│  
│   └── 02_Ticket_Sales_Forecast.ipynb  
│   Forecasting models for theatre ticket sales  
│
├── src  
│   Reusable Python functions for forecasting and analysis  
│
├── data  
│   Documentation of expected dataset structure (raw data not included)  
│
└── outputs  
    Generated figures and analysis outputs
    
## Workflow

1. Assess booking curve predictability using **AMI analysis**.
2. Use insights from forecastability diagnostics to design forecasting features.
3. Train and evaluate forecasting models using booking curve features.

4. ## Data Availability

The dataset used in this project contains internal ticketing data and is not included in this repository.

The notebooks assume access to a dataset containing the variables listed above.
    
