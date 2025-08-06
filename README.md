# ☕ Coffee Machine Simulation in Python

A simple console-based Coffee Machine program written in Python that simulates ordering and making coffee (Espresso, Latte, Cappuccino). It handles ingredient resources, accepts coins, calculates change, and gives reports.

---

## 📌 Features

- Select from 3 coffee types: **Espresso**, **Latte**, **Cappuccino**
- Simulates inserting coins and calculating total amount
- Handles:
  - Insufficient ingredients
  - Not enough money
  - Refund logic
- Shows a **report** of available ingredients and money
- Fully interactive **while loop** system with stop command

---

## 🛠️ Technologies Used

- Python 3
- Console-based input/output
- Basic conditionals, functions, and loops

---

## ▶️ How to Run

1. Make sure you have Python 3 installed.
2. Copy the code into a file named `coffee_machine.py`
3. Run the script:
4. 
python coffee_machine.py

---

## 📄 Resources and price
<pre>
  
| Drink      | Water (ml) | Coffee (g) | Milk (ml) | Price (\$) |
| ---------- | ---------- | ---------- | --------- | ---------- |
| Espresso   | 50         | 18         | 0         | 1.5        |
| Latte      | 200        | 24         | 150       | 2.5        |
| Cappuccino | 250        | 24         | 100       | 3.0        |

</pre>
---

## 💰 Coin System

- When prompted, you insert coins:

  Quarters = $0.25

  Dimes = $0.10

  Nickels = $0.05

  Pennies = $0.01

- The program calculates total amount inserted and gives change if overpaid, or refunds if underpaid.

---

## 📄 Example Usage

<pre>
  
What would you like? (espresso/latte/cappuccino): espresso
Please insert coins.
How many quarters: 10
How many dimes: 10
How many nickles: 10
How many pennies: 10
Here is $2.6 in change
Enjoy your espresso 👍
What would you like? (espresso/latte/cappuccino): latte
Please insert coins.
How many quarters: 10
How many dimes: 10
How many nickles: 5
How many pennies: 10
Here is $1.35 in change
Enjoy your latte 👍
What would you like? (espresso/latte/cappuccino): stop
  
</pre>

---

##📋 Future Improvements

- Add GUI using tkinter

- Log order history

- Add refill option for ingredients

- Add user accounts for loyalty points

---

## ✅ Learning Highlights

- Function design and parameter passing

- Input handling and user interaction

- Conditional checks and validation

- Basic money calculations

- Modular and readable code structure

