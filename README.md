# 🛒 Discount Calculator

This is a simple Python program that calculates the final price of an item after applying a discount.  
If the discount percentage is **20% or higher**, the discount is applied. Otherwise, the original price is returned.

---

## 📌 Features
- Takes the **original price** and **discount percentage** as input.
- Applies the discount only if it is **20% or higher**.
- Prints the final price after applying the discount.
- Handles invalid inputs gracefully.

---

## 🖥️ How to Run

1. Clone or download this project to your computer.
2. Make sure you have **Python 3** installed.
3. Open a terminal in the project directory.
4. Run the program with:

```bash
python discount_calculator.py
```
This is how and where you will enter your input and receive your output:

```bash
Enter the original price of the item: 1000
Enter the discount percentage: 25
Final price after 25% discount: 750.00
```
If the discount is less than 20%:
```

Enter the original price of the item: 1000
Enter the discount percentage: 10
No discount applied. Final price: 1000.00
```
Here is the function details that makes the discount to happen:
```
def calculate_discount(price, discount_percent):
    """Calculate final price after discount if discount >= 20%"""
    if discount_percent >= 20:
        discount_amount = (discount_percent / 100) * price
        final_price = price - discount_amount
        return final_price
    else:
        return price
```

🚀 Future Improvements

1. Add input validation for negative numbers.
2. Allow multiple items with different discounts.
3. Build a simple GUI for easier usage.

💡 Author: Innocent Akumu Omollo

