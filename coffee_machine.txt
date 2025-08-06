def calc_bill():
    print("Please insert coins.")
    quarters=int(input("How many quarters: "))
    dimes=int(input("How many dimes: "))
    nickles=int(input("How many nickles: "))
    pennies=int(input("How many pennies: "))
    quarter=0.25
    dime=0.10
    nickle=0.05
    pennie=0.01
    q=quarter*quarters
    d=dime*dimes
    n=nickle*nickles
    p=pennie*pennies
    sum=q+d+n+p
    return sum


def espresso(water,coffee,money):
    if water>=50 and coffee<18:
        print("sorry there is not enough coffee")
    elif water<50:
        print("sorry there is not enough water")
    elif water<50 and coffee<18:
        print("sorry there is not enough water and coffee")
    elif water>=50 and coffee>=18:
        water-=50
        coffee-=18
        price=1.5
        money_taken=calc_bill()
        change=money_taken-price
        if change>=0:
         money+=price
         print(f"Here is ${round(change,3)} in change")
         print("Enjoy your espresso 👍")
        elif change<0:
         print("Sorry thats not enough money. Money is refunded")
    return water,coffee,money     
    
def latte(water,coffee,milk,money):
    if water<200:
        print("sorry there is not enough water")
    elif coffee<24:
        print("sorry there is not enough coffee")
    elif milk<150:
         print("sorry there is not enough milk")
    elif water>=200 and coffee>=24 and milk>=150:
        water-=200
        coffee-=24
        milk-=150
        price=2.5
        money_taken=calc_bill()
        change=money_taken-price
        if change>=0:
         money+=price
         print(f"Here is ${round(change,3)} in change")
         print("Enjoy your latte 👍")
        elif change<0:
         print("Sorry thats not enough money. Money is refunded")
    return water,coffee,milk,money
    
def cappuccino(water,coffee,milk,money):
    if water<250:
        print("sorry there is not enough water")
    elif coffee<24:
        print("sorry there is not enough coffee")
    elif milk<100:
         print("sorry there is not enough milk")
    elif water>=250 and coffee>=24 and milk>=100:
        water-=250
        coffee-=24
        milk-=100
        price=3
        money_taken=calc_bill()
        change=money_taken-price
        if change>=0:
         money+=price   
         print(f"Here is ${round(change,3)} in change")
         print("Enjoy your cappuccino 👍")
        elif change<0:
         print("Sorry thats not enough money. Money is refunded")
    return water,coffee,milk,money

    
def report(water, coffee, milk, money):
 print(f"water: {water}")
 print(f"coffee: {coffee}")
 print(f"milk: {milk}")
 print(f"money: ${money}")



water=300
coffee=100
milk=200    
money=0


should_continue=True
while should_continue:
    user_input=input("What would you like? (espresso/latte/cappuccino): ").lower()
    if user_input=='espresso':
        water,coffee,money=espresso(water,coffee,money)
    elif user_input=='latte':
        water,coffee,milk,money=latte(water,coffee,milk,money)
    elif user_input=='cappuccino':
        water,coffee,milk,money=cappuccino(water,coffee,milk,money)
    elif user_input=='report':
        report(water, coffee, milk, money)
    elif user_input=='stop':
        should_continue=False
