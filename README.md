
# Credit Card Offer Analysis

Inflation, Inflation, Inflation… Despite the grim economic outlook, people still need to buy, and companies still need to sell. Or at least try to get you to spend more. Among those strategies by companies to get you to buy more are credit cards.

Credit card offers can be attractive, but depending on the credit card and how you use, it can either bring in some cash or worsen your credit score. The question is, how can you be smart about with your money?

In this project I analyse my credit card expenses and purchasing habits to determine if a credit offer I got is worth accepting.

![image](https://github.com/aleivaar94/BMO-Airmiles-Analysis/blob/master/images/credit-card-cbc-news.png)


# Methodology

Air Miles are awarded depending on the amount spent. The normal rate is 1 mile for every $20.0 dollars. However, if you use a credit card from a bank affiliated with Air Miles you can earn more Air Miles with less money spent. Certain stores give more miles than the standard rate. For example, Safeway gives 3x more miles.

- Standard Air Miles: 1 miles for every $20.0 spent.
- BMO *Air Miles* Mastercard: 3 miles for every $25.0 spent.
- BMO *Air Miles World Elite* Mastercard: 3 miles for every $12.0 spent.

Conversion of miles to cash:

95 miles = $10.0 or,

9.5 miles = $1.0

![image](https://github.com/aleivaar94/BMO-Airmiles-Analysis/blob/master/images/bmo-airmiles-offer.png)

## Data Collection

I track my expenses and keep them in an Excel spreadsheet. Each expenses includes information such as data, amount, category, store, etc. 

![image](https://github.com/aleivaar94/BMO-Airmiles-Analysis/blob/master/images/df-expenses.png)


## Data Analysis

1. Air Miles are then calculated from credit card purchases, excluding purchases made with debit or any other form of payment that would not give air miles in return. Affiliated stores that give more air miles than the standard rate are taking into account.
2. The amount of each expense is divided by a floor division so that every $20.0 dollars gives 1 mile, $40.0 dollars 2 miles and so on.
3. Extra miles are calculated for affiliated stores that give more miles than the standard rate of 1 mile = $20.0 dollars.
4. Miles are summed per year and the total cashback is calculated by subtracting the annual fee of each credit card.


# Results

![image](https://github.com/aleivaar94/BMO-Airmiles-Analysis/blob/master/images/df-benefits-cards.png)

In 2021, with the BMO Elite card I could have earned almost $300.0 dollars worth for miles or $111.0 dollars more than my current Scotiabank cash back card.

In 2022 the BMO Elite card still doesn't bring me benefit. In fact, I would have earned $167 instead of $181 dollars currently earned with my Scotia card. However, the year is not over, and I will accumulate more purchases which will make the BMO Elite card bring me more cash back by the end of the year.

# Conclusion

The BMO Air Miles World Elite credit card is a good option offered and I should consider switching to it, because it is better than the Scotiabank cash back credit card I currently have. 


## 🔗 Links
[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://alejandroleiva.notion.site/Data-Portfolio-5c5257235e044c6b9a8846131edac973)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ale-leivaar/)
