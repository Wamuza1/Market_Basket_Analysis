# Market_Basket_Analysis

# Python

## Theory of Apriori Algorithm

There are three major components of Apriori algorithm:

- Support
- Confidence
- Lift

### Suppose 

we have a record of 1 thousand customer transactions, and we want to find the Support, Confidence, and Lift for two items e.g. burgers and ketchup. Out of one thousand transactions, 100 contain ketchup while 150 contain a burger. Out of 150 transactions where a burger is purchased, 50 transactions contain ketchup as well. Using this data, we want to find the support, confidence, and lift. 

Support Support refers to the default popularity of an item and can be calculated by finding number of transactions containing a particular item divided by total number of transactions. Suppose we want to find support for item B. This can be calculated as:
![image](https://user-images.githubusercontent.com/92646311/205537407-7d619c79-94cc-4766-8545-65a558ee1a4a.png)

For instance if out of 1000 transactions, 100 transactions contain Ketchup then the support for item Ketchup can be calculated as:
![image](https://user-images.githubusercontent.com/92646311/205537475-9b6484d9-2171-4630-a445-319de7ecdf21.png)

### Confidence

Confidence refers to the likelihood that an item B is also bought if item A is bought. It can be calculated by finding the number of transactions where A and B are bought together, divided by total number of transactions where A is bought. Mathematically, it can be represented as:
![image](https://user-images.githubusercontent.com/92646311/205537576-cb9d1e73-0ed1-4411-ae35-b7a15038f58c.png)

Coming back to our problem, we had 50 transactions where Burger and Ketchup were bought together. While in 150 transactions, burgers are bought. Then we can find likelihood of buying ketchup when a burger is bought can be represented as confidence of Burger -> Ketchup and can be mathematically written as:
![image](https://user-images.githubusercontent.com/92646311/205537635-f7d4e334-ebc0-4a07-8134-0a9fcbe40944.png)

###Lift

Lift(A -> B) refers to the increase in the ratio of sale of B when A is sold. Lift(A –> B) can be calculated by dividing Confidence(A -> B) divided by Support(B). Mathematically it can be represented as:
![image](https://user-images.githubusercontent.com/92646311/205537737-4d2cb8df-ef37-4016-bed8-ceb44d262e79.png)

Coming back to our Burger and Ketchup problem, the Lift(Burger -> Ketchup) can be calculated as:
Lift basically tells us that the likelihood of buying a Burger and Ketchup together is 3.33 times more than the likelihood of just buying the ketchup. A Lift of 1 means there is no association between products A and B. Lift of greater than 1 means products A and B are more likely to be bought together. Finally, Lift of less than 1 refers to the case where two products are unlikely to be bought together.
![image](https://user-images.githubusercontent.com/92646311/205537798-e64a4bf7-923d-47da-bafb-414cd8895e15.png)


# R


### Numers of observations and variables.

![image](https://user-images.githubusercontent.com/92646311/205535103-680869eb-e286-4151-9752-9847bc8054f3.png)

### Data  structure.

![image](https://user-images.githubusercontent.com/92646311/205535298-295d1adf-2e37-4e7a-b60f-cb62f611d014.png)

### Package ‘arules’ Documentation:

Provides the infrastructure for representing, manipulating and analyzing transaction data and patterns (frequent itemsets and association rules). Also provides C implementations of the association mining algorithms Apriori and Eclat. Hahsler, Gruen and Hornik (2005) <doi:10.18637/jss.v014.i15>.

https://cran.r-project.org/web/packages/arules/arules.pdf

