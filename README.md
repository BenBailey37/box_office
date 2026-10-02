#Judson Box Office
print("Welcome to the Judosn Box Office")
total_sales = 0.00

costomers = []
sales = []

#Ask for costomer's name
name = input("Costomer name (or done):  ")
while name != "done":
	age = int(input("Age: "))
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
	for ticket in range(1, quantity + 1):
        	print(f"Ticket {ticket} / {quantity}: ${price:.2f}")

#name pays subtotal
	subtotal = price * quantity
	subtotal = int(subtotal)
	total_sales = total_sales + subtotal
	print(f"{name} pays ${subtotal:.2f}")
	name = input("Costomer name (or done):  ")
	costomers.append(name)
	sales.append(subtotal)
#has problem!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
print(f"Closed. Total sales: ${total_sales:.2f}")
print("Costomers served: ", len(costomers))
print(sales)

#while name is not done:
	#ask age, quantity, deside price
	#show hello; for tickets show line
	#set subtotal
	#add subtotal to total_sales
	#show name pays subtotal
	#ask the next name (or done)
#show closed. total sales

