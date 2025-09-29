# Banking-Dashboard

[Click Here to get Dataset](https://github.com/KishoreKonkena/Banking-Dashboard/blob/main/Banking.xlsx).

![Banking Logo](https://github.com/KishoreKonkena/Banking-Dashboard/blob/main/Screenshot%202025-09-29%20110216.png)

**Problem Statement** –

Develop a basic understanding of risk analytics in banking and financial services and understand how data is used to minimise the risk of losing money while lending to customers.

**Solution** – 

With our dashboards which are created using Power BI latest tools helps the company to make a decision based on the applicant’s profile like if the applicant is likely to repay the loan then approving the loan otherwise not.

**About Dataset** – 

This dataset basically contains information about bank details ,various client details which consists of multiple tables which are interlinked with each other through keys like primary key and foreign key.
The various tables are Banking Relationship, Client-Banking, Gender, Investment Advisor and Period.

**Calculated Functions** – 

**Sum** : 

The power bi sum function will add all the numbers in a column and the column contains numbers to sum. It returns a decimal number.

**Syntax** :

Sum= SUM(<column>)

**Example**:

Bank Deposit = 
SUM('Bank Clients'[Bank Deposits] )

**DistinctCount** :


Counts the number of distinct values in a column


**Syntax**:


DISTINCTCOUNT(<column>)


Example :


Total Clients = DISTINCTCOUNT('Bank Clients'[Client ID] )

**Sumx :**


Returns the sum of an expression evaluated for each row in a table.


**Syntax**:


SUMX(<table>, <expression>)


**Example** :

Total Fees = SUMX('Bank Clients' , [Total Loan] * 'Bank Clients'[Processing Fees] )

**Switch :**


Evaluated an expression against a list of values and returns one of multiple possible result expressions


**Syntax :**


SWITCH(<expression>, <value>, <result>[, <value>, <result>]…[, <else>])

**DATEDIFF :**


Returns the number of interval boundaries between two dates.


**Syntax :**


DATEDIFF(<Date1>, <Date2>, <Interval>)

**Example :**


Engagment Days = DATEDIFF('Bank Clients'[Joined Bank],TODAY(), DAY )

**KPI’S:** 

In which followings KPIS are present :

**Total Clients** : 


Total Clients KPI represents total number of clients in banking.


Total Clients = DISTINCTCOUNT('Bank Clients'[Client ID] )

![Total Clients](https://github.com/KishoreKonkena/Banking-Dashboard/blob/main/cards/Screenshot%202025-09-29%20113728.png)


**Total Loan :**


Total Loan gives you information about the bank loan + Business lending + credit cards balance of particular  investor , gender.


Total Loan = [Bank Loan] + [Business Lending] + [Credit Cards Balance]

![Total Loan](https://github.com/KishoreKonkena/Banking-Dashboard/blob/main/cards/Screenshot%202025-09-29%20114051.png)


**Bank Loan :**

Bank Loan gives you information what is the loan amount of loan to be repaid by the client to bank.

Bank Loan = SUM('Bank Clients'[Bank Loans] )

![Bank Loan](https://github.com/KishoreKonkena/Banking-Dashboard/blob/main/cards/Screenshot%202025-09-29%20114324.png)

**Business Lending :**

Business lending gives you information about the loan amount given to small business.

Business Lending = SUM('Bank Clients'[Business Lending] )

![Business Lending](https://github.com/KishoreKonkena/Banking-Dashboard/blob/main/cards/Screenshot%202025-09-29%20114533.png)

**Total Deposit :**

Total Deposit gives you information about the amount deposited by particular investors in bank

Total Deposit = [Bank Deposit] + [Savings Account] + [Foreign Currency Account] + [Checking Accounts]

![Total Deposit](https://github.com/KishoreKonkena/Banking-Dashboard/blob/main/cards/Screenshot%202025-09-29%20114741.png)

**Bank Deposit :**

Bank deposit is the money put in the bank.

Bank Deposit = 

SUM('Bank Clients'[Bank Deposits] )

![Bank Deposit](https://github.com/KishoreKonkena/Banking-Dashboard/blob/main/cards/Screenshot%202025-09-29%20115017.png)


**Checking Account Amount :**

Checking account amount  is nothing but which offers easy access to your money for daily transactional needs.

Checking Accounts = 

SUM('Bank Clients'[Checking Accounts] )

![Checking account amount](https://github.com/KishoreKonkena/Banking-Dashboard/blob/main/cards/Screenshot%202025-09-29%20115652.png)

**Total CC Amount :**

Total CC Amount is a short-term source of financing for a company by a bank.

Total CC Amount = SUM('Bank Clients'[Amount of Credit Cards] )

![Total CC Amount](https://github.com/KishoreKonkena/Banking-Dashboard/blob/main/cards/Screenshot%202025-09-29%20115939.png)

**Saving Account Amount :**

A savings account is an interest-bearing deposit account held at a bank.

Savings Account = SUM('Bank Clients'[Saving Accounts] ) 

![Total savings account](https://github.com/KishoreKonkena/Banking-Dashboard/blob/main/cards/Screenshot%202025-09-29%20120140.png)

**Foreign Currency Amount :**

Foreign Currency Account means an account held in a currency that is not the currency of India or Bhutan or Nepal.

Foreign Currency Account = 

SUM('Bank Clients'[Foreign Currency Account] ) 

![Total Foreign Currency Account](https://github.com/KishoreKonkena/Banking-Dashboard/blob/main/cards/Screenshot%202025-09-29%20120355.png)

**Credit Cards Balance :**

It is the total amount of money currently owned by a cardholder to their credit card bank.

Credit Cards Balance = SUM('Bank Clients'[Credit Card Balance] )



**Visualization And Result –**

**Home**

![Home Dashboard](https://github.com/KishoreKonkena/Banking-Dashboard/blob/main/cards/Screenshot%202025-09-29%20121039.png)

**Loan Analysis**

![Loan Analysis Dashboard](https://github.com/KishoreKonkena/Banking-Dashboard/blob/main/cards/Screenshot%202025-09-29%20121358.png)

**Deposit Analysis**

![Deposit Analysis Dashboard](https://github.com/KishoreKonkena/Banking-Dashboard/blob/main/cards/Screenshot%202025-09-29%20121551.png)

**Summary Dashboard**

![Summary Dashboard](https://github.com/KishoreKonkena/Banking-Dashboard/blob/main/cards/Screenshot%202025-09-29%20121747.png)


**Conclusion –**

Empowered by the latest data visualization techniques, Power BI dashboards are among the most effective resources for using in banking sector. As outlined in this write-up, a banking  operations dashboard in Power BI can be developed with key banking related metrics and KPIs.

**Future Work –**

With these dashboards banks can easily know what is the total loan amount and all other things of a particular investor.
It also helps which type of banks have more number of clients as we can see private banks have more number of clients so it can helps other banks can build their strategies to increase clients.
It also provides insights about which nationality has highest bank loans.
It gives information about various types of amount involved in different types of accounts by investors.







































