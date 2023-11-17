# OOAD-CaseStudy
## Class Diagram
![Screenshot (52)](https://github.com/abrahamjk15/OOAD-CaseStudy/assets/58914169/c97a104d-f8fb-44cf-b3e7-35d6679ffbcb)

### Domain: Banking

Use case : When a customer attempts to deposit money, the list of all accounts which the customers possess should be listed so that the customer can select to which account he would like to deposit the money.[Hint: Customer has Accounts] . Customer can have the following accounts

SavingsMaxAccount

CurrentAccount

LoanAccount

- Customer(customerCode,customerName,List<Account>)

- Account(accountNo,accountType,balance,Product).

- Product(productCode,productName,List<Service>)

- SavingsMaxAccount is a Product(minimumBalance of Rs1000 should be maintained in the account)

- CurrentAccount is a Product

- LoanAccount is a Product.(chequeDeposit should be chargeable ie).3%).

- Service(serviceCode,serviceName,rate)

He should be given default services like

SavingsMaxAccount(CashDeposit. ATMWithdrawl,OnlineBanking)

CurrentAccount(CashDeposit,OnlineBanking,ATMWithdrawl,MobileBanking)

LoanAccount(CashDeposit,ChequeDeposit)
