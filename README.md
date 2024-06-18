# Atmpythonproject
import time
print("please insert your card")
time.sleep(5)
password=1234
pin=int(input("enter your pin:"))

balance=5000
Account_number=1234567890
phone_number=9876543210
otp=2011
if pin==password:
          while True:

                    print("""
                              1 == Current abalance
                              2 == Withdraw Amount 
                              3 == Deposit Amount
                              4 == Pin Generation
                              5 == exit
                              """
                              )
                    try:
                              option=int(input("Enter your option"))
                    except:
                              print("please enter valid option")
                              
                    if option == 1:
                              print(f"your current balance is{balance}")
                              
                    if option == 2:
                              Withdraw_amount=int(input("please enter Withdrawal amount"))
                              balance=balance-Withdraw_amount
                              print(f"{Withdraw_amount} is debited from your account")
                              print(f"your updated balance is{balance}")
                              
                    if option == 3:
                              Deposit_amount=int(input("enter deposit_amount"))
                              balance =balance + Deposit_amount
                              print(f"your updated balance is{balance}")
                    if option == 4:
                        acc_number=int(input("Enter account number"))
                        if acc_number == Account_number:
                                phn_number=int(input("Enter phone number :"))
                                if phn_number == phone_number :
                                        otp_number=int(input("Enter otp :"))
                                        if otp_number == otp :
                                                Password=int(input("Enter new password"))
                                                print("Password created successfully....")
                                        else:
                                                print("Enter valid otp")
                                else:
                                        print("Enter valid phone number")
                        else:
                                print("Enter valid account number")
                    if option == 5:
                            break
else:
        print("wrong pin please try again")
