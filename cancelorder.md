#Code to cancel the order in the Online Shopping Database
def cancelOrder():
    found = False
    temp = &#91;]
    order_id = input("Enter the order id : ")
    for d in shopping:
        found = d&#91;"id"] == order_id
        if found != True:
            temp.append(d)
    if len(temp) == d:
        print(f'{order_id} is not found')
    else:
        print(f'{order_id} is removed from the placed order')
        
