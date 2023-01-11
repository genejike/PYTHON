#If the bill was $150.00, split between 5 people, with 12% tip. 

    message ='Welcome to the tip calculator'
    print(message)

#Each person should pay (150.00 / 5) * 1.12 = 33.6

    bill =int(input("what was the total bill? $"))
    tip_given=int(input("what percentage tip would you like to give?10,12 and 15?"))
    bill_split = int(input("how many people to split bill?"))
    tip =round((bill / bill_split) * (1+(tip_given/100)),2)
    message_2 = f"Each person should pay:${tip}"

    print ( message_2 )

![Alt text](images/tip%20calculator.png)