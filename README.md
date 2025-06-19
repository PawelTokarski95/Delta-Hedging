# Delta-Hedging

- **Language**: Python

1. What is Delta Hedging?
   
Delta hedging is a method used to protect an investment portfolio. It works by making opposite trades in two different financial products: options and the underlying stock. There are two main types of options:
Call option – gives the right to buy the stock.
Put option – gives the right to sell the stock.
The delta tells us how much the option price will change if the stock price changes. For call options, delta is between 0 and 1 and for put options, delta is between –1 and 0.
When the price of the stock goes up:
Call option becomes more valuable,
Put option becomes less valuable.
But the change is not identical. The option price moves slower or faster than the stock, depending on the situation. To hedge your position, you need to buy or sell shares to cancel this risk.

3. Option pricing
   
I calculated the prices of call options for 7 different stocks using the Black-Scholes model.
This model makes a few simple assumptions about the market:
-No transaction costs,
-No no arbitrage,
-Stock returns follow a normal distribution.
Although the model is not perfect, many banks and traders use it as a first step to estimate option prices.

![448393374-7ed80826-1a20-4657-9f12-1139a5090c19](https://github.com/user-attachments/assets/5b3cfbed-c577-4d4e-9f35-4b3c74aa5a82)


5. Delta Hedging

After calculating the option prices and deltas, I used delta hedging:
I took an opposite position in the stock to reduce the risk from the option.
Example:
If the option delta is 0.6, I sold 0.6 shares of the stock for every option I held.
This made the portfolio delta-neutral – meaning it’s protected from small price changes in the stock.


4. Results of the Strategy
   
The results showed that delta hedging worked pretty good.
In most cases, the portfolio’s delta was dropping significantly, meaning the price risk was much lower.



![delta hedge 1](https://github.com/user-attachments/assets/845b50b4-eac4-4414-afd1-673f28266ad0)


![delta hedge 2](https://github.com/user-attachments/assets/a828a1e5-fcc9-4aaa-a534-d22217be796f)


![delta hedge  6](https://github.com/user-attachments/assets/f1524318-0da4-4310-b477-a6981c989510)

![delta hedge  5](https://github.com/user-attachments/assets/e51f97df-ed28-4c67-9311-e517073a4060)

![delta hedge  4](https://github.com/user-attachments/assets/7330e78d-107e-4f6e-a75e-f4e19bd4950b)

![delta hedge  3](https://github.com/user-attachments/assets/2247aee5-07de-4448-8dc3-65c15526a22f)

![delta hedge  7](https://github.com/user-attachments/assets/9c79fef6-1526-43ed-9517-972c7a4da2e4)
