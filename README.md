# Basic Microservices exchange and conversion

Repository with Docker files configurations for setting up microservices. 

## Prerequisites

- Docker

## Exchange Service

The Exchange Service provides currency values like:

- 1 USD = 60 INR
- 1 AUD = 50 INR. 

## Currency Conversion

The Currency Conversion Service converts amounts by fetching exchange rates. For example, to convert 10 USD, it gets the rate of 1 USD (60 INR) from the Exchange Service and multiplies to get 600.

## Usage

1. Clone this repository to your local machine:
   ```sh
   git clone 
   cd microservices-docker-compose
   
2. Execute docker-compose
   ```sh
   docker-compose up

3. Verify the web

   Exchange: http://localhost:8000/currency-exchange/from/EUR/to/INR

   ![image](https://github.com/user-attachments/assets/4fa16fbe-fb59-499c-8dfd-91d145d14716)

   Conversion: http://localhost:8100/currency-conversion/from/EUR/to/INR/quantity/
   
   ![image](https://github.com/user-attachments/assets/468abbd7-6477-4e8f-961f-7deece3e06fd)
   
4. Dockerhub
   You can also check the repositories in dockerhub
   ![image](https://github.com/user-attachments/assets/09f128a0-03d6-44a0-91f9-a47c63e0bbe5)

   Verify the Dockerfiles used for the exchange and conversion repositories in dockerhub
   
   ```sh
   cd conversion-dockerfile
   cd exchange-dockerfile

   

   
