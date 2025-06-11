# Delta-Hedging

1. What is Delta Hedging?
   
Delta hedging is a method used to protect an investment portfolio. It works by making opposite trades in two different financial products: options and the underlying stock (the stock the option is based on). There are two main types of options:
Call option – gives the right to buy the stock
Put option – gives the right to sell the stock
The delta tells us how much the option price will change if the stock price changes. For call options, delta is between 0 and 1 For put options, delta is between –1 and 0
When the price of the stock goes up:
Call option becomes more valuable
Put option becomes less valuable
But the change is not 1-to-1. The option price moves slower or faster than the stock, depending on the situation. To hedge (protect) your position, you need to buy or sell shares to cancel out this risk.

3. How I Priced the Options
   
I calculated the prices of call options for 7 different stocks using the Black-Scholes model.
This model makes a few simple assumptions about the market, like:
-No transaction costs
-No risk-free profits (no arbitrage)
-Stock returns follow a normal distribution.
Even though the model is not perfect, many banks and traders use it as a first step to estimate option prices.

5. What I Did – Delta Hedging

After calculating the option prices and deltas, I used delta hedging:
I took an opposite position in the stock to reduce the risk from the option.
Example:
If the option delta is 0.6, I sold 0.6 shares of the stock for every option I held.
This made the portfolio delta-neutral – meaning it’s protected from small price changes in the stock.


Simple Example – For Beginners

Let’s say you have 1 call option on Apple stock.
Apple stock price = $100
Option delta = 0.5
This means:
The option will go up by about $0.50 if Apple’s stock goes up by $1. To protect yourself, you sell 0.5 shares of Apple
If Apple’s stock goes up $1:
You gain $0.50 on the option
You lose $0.50 on the stock
Net effect: zero

That’s how delta hedging works. It protects you from small changes in stock price.


4. Results of the Strategy
   
The results showed that delta hedging worked well.
In most cases, the portfolio’s delta was dropping significantly, meaning the price risk was much lower.



![delta hedge 1](https://github.com/user-attachments/assets/845b50b4-eac4-4414-afd1-673f28266ad0)


![delta hedge 2](https://github.com/user-attachments/assets/a828a1e5-fcc9-4aaa-a534-d22217be796f)


![delta hedge  6](https://github.com/user-attachments/assets/f1524318-0da4-4310-b477-a6981c989510)

![delta hedge  5](https://github.com/user-attachments/assets/e51f97df-ed28-4c67-9311-e517073a4060)

![delta hedge  4](https://github.com/user-attachments/assets/fd64d33a-14bb-49a8-9441-6e763335aa9a)

![delta hedge  3](https://github.com/user-attachments/assets/2247aee5-07de-4448-8dc3-65c15526a22f)

![delta hedge  7](https://github.com/user-attachments/assets/9c79fef6-1526-43ed-9517-972c7a4da2e4)
