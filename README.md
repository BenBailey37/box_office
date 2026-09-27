#Judson Box Office
print("Welcome to the Judosn Box Office")
total_sales = 0

#Ask for costomer's name
name = input("What is your name? ")
age = int(input("Age: "))
#ask how many tickets
quantity = int(input("How many tickets? "))

#pricing: under 5 free, under 18, $8, 65+ $10, else $12
if age < 5:
        price = 0.00
elif age < 18:
        price = 8.00
elif age >= 65:
        price = 10.00
else:
        price = 12.00

print(f"Hello, {name}")
#show ticket of price
for ticket in range(1, quantity + 1):
        print(f"Ticket {ticket} of {quantity}: ${price:.2f}")

#name pays subtotal
subtotal = price * quantity
print(f"{name} pays ${subtotal:.2f}")

total_sales = (total_sales + subtotal)

#set total sales = 0 DONE
#ask first name (or done)
#while name is not done:
	#ask age, quantity, deside price
	#show hello; for tickets show line
	#set subtotal
	#add subtotal to total_sales
	#show name pays subtotal
	#ask the next name (or done)
#show closed. total sales
