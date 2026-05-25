

# Students-ATM. Py
#The ATM is to help students manage their finances.
print () 
balance = 1000
while True:
    print("\n1. Check balance")
    print("2. Deposit cash")
    print("3. Withdraw cash")
    print("4. Goodbye!")

    choice = input("Choose option: ")

    ############################
    if choice == "1":
        print(f"Your balance is: {balance}")

    ############################
    elif choice == "2":
        amount = int(input("Enter amount to deposit: "))
        balance = balance + amount
        print(f"Deposited! New balance: {balance}")

    ############################
    elif choice == "3":
        amount = float(input("Enter amount to withdraw: "))

        if balance < amount:
            print("Insufficient funds")

        else:
            balance = balance - amount
            print(f"New balance: {balance}")

    ############################
    elif choice == "4":
        print("Goodbye!")
        break

    ############################
    else:
        print("Invalid choice")
