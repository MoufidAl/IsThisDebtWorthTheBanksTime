# Is This Deb tWorth The Bank's Time and Effort?
Regression Discontinuity Analysis to conclude whether certain debts are worth the bank's time and effort to pursue? especially since each extra level of recovery possibility costs the bank an extra 50$ per customer

## Background Information
After a debt has been legally declared "uncollectable" by a bank, the account is considered "charged-off." But that doesn't mean the bank <strong><em>walks away</em></strong> from the debt. They still want to collect some of the money they are owed. The bank will score the account to assess the expected recovery amount, that is, the expected amount that the bank may be able to receive from the customer in the future. This amount is a function of the probability of the customer paying, the total debt, and other factors that impact the ability and willingness to pay.</p>
<p>The bank has implemented different recovery strategies at different thresholds (\$1000, \$2000, etc.) where the greater the expected recovery amount, the more effort the bank puts into contacting the customer. For low recovery amounts (Level 0), the bank just adds the customer's contact information to their automatic dialer and emailing system. For higher recovery strategies, the bank incurs more costs as they leverage human resources in more efforts to obtain payments. Each additional level of recovery strategy requires an additional \$50 per customer so that customers in the Recovery Strategy Level 1 cost the company \$50 more than those in Level 0. Customers in Level 2 cost \$50 more than those in Level 1, etc.

## The Goal of this Analysis
Does the extra amount that is recovered at the higher strategy level exceed the extra \$50 in costs? In other words, was there a jump (also called a "discontinuity") of more than \$50 in the amount recovered at the higher strategy level?

## Methods / Tools utilized
* pandas
* NumPy
* Graphical Exploratory Analysis (matplotlib)
* scipy
* Statistical tests: (kruskal), chi-square
* statsmodels.api 
* regression analysis

## Conclusion
Whether I use a wide (\$900 to \$1100) or narrower window (\$950 to \$1050), the incremental recovery amount at the higher recovery strategy is much greater than the \$50 per customer it costs for the higher recovery strategy.  So I conclude that the higher recovery strategy is worth the extra cost of \$50 per customer.

## Credits
The dataset can be found on Datacamp.com
Project was completed without any assistance, hints, or help from any entity or person.
