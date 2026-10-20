# Electricity Bill calculator
## This program calculates the electricity consumption and total bill.
## Version 1 - Original code without input validation
- Input: Accepts a name, previous, and current meter reading.
- Process: Calculates and displays the name, consumption, and total bill.
- Output: consumption, name, and total bill.
- Does not include input validation.

# Electricity Bill Calculator
RATE = 12.90
name = input("Enter customer name: ")
previous = float(input("Enter previous meter reading: "))
current = float(input("Enter current meter reading: "))

consumption = current - previous
total_bill = consumption * RATE

print("\nCustomer:", name)
print("Electricity Consumption:", consumption, "kWh")
print("Total Bill: PHP", round(total_bill, 2))

# Validation rules
# 1. Customer name -- Must not be empty
# 2. Previous reading -- Number at least 0
# 3. Current reading -- Number at least the previous reading
