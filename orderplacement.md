# Online-Shopping-Database
A program that allows you to shop online and track your order. 
#Code to place an order in Online Shopping Database

def placeOrder():
    order_number = 10
    userDisplayMenuWindow()
    p_id = int(input("\nEnter the id : "))

    for d in shopping:
        if d&#91;"id"] == p_id:
            print("\nId\tName\tAvailable\tPrice")
            print("=============================================================")
            print(f'{d&#91;"id"]}\t{d&#91;"Name"]}\t{d&#91;"Available"]}\t\t{d&#91;"Price"]}')
            order = '{d&#91;"id"]}\t{d&#91;"Name"]}\t{d&#91;"Available"]}\t\t{d&#91;"Price"]}'
            conform = input("\nDo you want to place an order on the above shown product : Y/N ")

            if conform == 'Y' or conform == 'y':
                print("\nSuccessfully placed the order on the product {} {}".format(d&#91;"id"], d&#91;"Name"]))
                order_number += 1
                print("Your order number is : ", order_number)
                d&#91;"Available"] -= 1
                break

            elif conform == 'N' or conform == 'n':
                print("The order is not placed. You can carry on with you purchase. Happy shopping!!!!")
                break
            else:
                print("\nYou have entered wrong option. Please enter again\n")
                conform = input("\nDo you want to place an order on the above shown product : Y/N ")
                break

    if d&#91;"id"] != p_id:
        print("\nYou have entered invalid id. Please enter valid id\n")
        user_id()
    print("\nAvailable products : \n")
    userDisplayMenuWindow()

def placeOrder():
    order_number = 10
    userDisplayMenuWindow()
    p_id = int(input("\nEnter the id : "))
 
    for d in shopping:
        if d&#91;"id"] == p_id:
            print("\nId\tName\tAvailable\tPrice")
            print("=============================================================")
            print(f'{d&#91;"id"]}\t{d&#91;"Name"]}\t{d&#91;"Available"]}\t\t{d&#91;"Price"]}')
            order = '{d&#91;"id"]}\t{d&#91;"Name"]}\t{d&#91;"Available"]}\t\t{d&#91;"Price"]}'
            conform = input("\nDo you want to place an order on the above shown product : Y/N ")
 
            if conform == 'Y' or conform == 'y':
                print("\nSuccessfully placed the order on the product {} {}".format(d&#91;"id"], d&#91;"Name"]))
                order_number += 1
                print("Your order number is : ", order_number)
                d&#91;"Available"] -= 1
                break
 
            elif conform == 'N' or conform == 'n':
                print("The order is not placed. You can carry on with you purchase. Happy shopping!!!!")
                break
            else:
                print("\nYou have entered wrong option. Please enter again\n")
                conform = input("\nDo you want to place an order on the above shown product : Y/N ")
                break
 
    if d&#91;"id"] != p_id:
        print("\nYou have entered invalid id. Please enter valid id\n")
        user_id()
    print("\nAvailable products : \n")
    userDisplayMenuWindow()
