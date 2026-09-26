#Judson Box Office
print("Welcome to the Judosn Box Office")

#Ask for costomer's name
name = input("What is your name? ")
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
        print(f"Ticket {ticket} of {quantity}: $(price:.2f")


subtotal = price * quantity
print(f"{name} pays ${subtotal:.2f}")


#ask how many tickets

#diside the price(already have)

#show hello name(already have)

#for tidket from 1 to quantity:
#show ticket of price

#name pays subtotal
