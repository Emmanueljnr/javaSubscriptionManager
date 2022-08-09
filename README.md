# javaSubscriptionManager
Store Subscription Service using Object Orientated Programming

Visit this link to see how the application runs : https://streamable.com/7qisun

This programme is written in Java, its main function is to serve as a subscription service for users/customers who wish to subscribe to offers/packages offered by an imaginary store called GAS (Games Acess Service).

Fundamentally, the application is written using all object oriented programing principles. 


#################################################################
Stage 1 - Gives the user the chance to get a package

The user is provided with 4 options to select at the beginning, ideally they start with option 1 which will allow them to start a subscription of their chosing. This stage will also take in discount codes, however the discount code must meet a certain criteria for example:
Rule 1 : The code must be 6 characters long
Rule 2 : The code must be in this exact format i.e 'JF19L5'
Rule 3 : The first two letters can be anything at all, as they serve no particular purpose to the code itself
Rule 4 : the middle two digits i.e '19' represent the year, therefore the discount code must be valid for that particlua year. 19 = 2019
Rule 5 : The fifth character should be a letter, but only two letters can be accepted. either 'L' or 'E' 
          'E' = January - June
          'L' = July - December
meaning that the letter will be validated and compared to the month that this code is provided by the user in order to make sure that the code is valid. i.e if the user makes an attempt to register for a package in August, then the appropriate letter for their code should be the letter 'L'
Rule 6 : The last digit in the discountCode represents the percentage of the discount. 
          This can only be a single digit. In this example, JF19L5 :
          we can extrapolate that this code was valid in 2019 within the months of July and December and it was a 5% off discount code.
          
          
  * Once an order/package has been purchased, the system will the write the users details to a text file (current.txt), using the Writer method.
  We will then read from this text file using the Scanner method in stage 2 of the application
    
    
########################################################################

Stage 2 - Allows the clients to look at their receipt

########################################################################

Stage 3 - Allows the client to view the subscriptions they have for any given month. This data will be printed out as a receipt

#######################################################################

Stage 4 - Allows the manager to search for a clients name in order to see if it exists within the cirrent.txt file.
