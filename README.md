# Week 3 Assignment

## Question 1
- Define a function `calculate_discount(price, discount_percent)`  
- The function should:  
  1. Check if the discount is **20% or higher**.  
  2. If true, calculate the discount amount and subtract it from the original price.  
  3. Return the final price.  
  4. If false, return the original price without any discount.  

### Python Code:
```python
def calculate_discount(price, discount_percent):
    """
    Calculates the final price after applying a discount.
    If the discount is 20% or higher, it is applied.
    Otherwise, the original price is returned.
    """
    if discount_percent >= 20:
        discount_amount = price * (discount_percent / 100)
        final_price = price - discount_amount
        return final_price
    else:
        return price
