User_Account_Balance = 30000.65
print(User_Account_Balance)
try:
    withdrawal_amount = int(input("How much money do you want to withdraw? "))

    if withdrawal_amount <= 1000:
        print("Sorry, the minimum withdrawal amount should be more than 1000.")
    elif withdrawal_amount >= 30000:
        print("Your withdrawal amount exceeds the available balance limit.")
    else:
        print("You have withdrawn", withdrawal_amount, "Rupees.")
except ValueError:
    print("Error: The withdrawal amount must be a valid integer. Decimal values and non-numeric characters are not accepted.")
