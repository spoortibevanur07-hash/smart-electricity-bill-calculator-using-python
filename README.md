# Smart Electricity Bill Calculator

A beginner-friendly Python console program that calculates an electricity bill from the customer's name, customer ID, and units consumed.

## Run the program

```bash
python smart_electricity_bill_calculator.py
```

## Program flow

1. `get_customer_details()` asks for the customer name and customer ID.
2. The function asks for electricity units and converts the input to an integer.
3. Negative units and invalid unit input are rejected, and the user is asked to try again.
4. `calculate_bill()` calculates the energy charge using progressive slabs:
	- First 100 units: ₹2 per unit
	- Units 101 to 200: ₹4 per unit
	- Units 201 to 500: ₹6 per unit
	- Units above 500: ₹8 per unit
5. A fixed service charge of ₹100 is added to the energy charge.
6. `display_bill()` prints the customer details, units consumed, energy charge, service charge, and final amount.

## Example calculation

For 250 units:

- First 100 units: `100 × ₹2 = ₹200`
- Next 100 units: `100 × ₹4 = ₹400`
- Remaining 50 units: `50 × ₹6 = ₹300`
- Energy charge: `₹900`
- Service charge: `₹100`
- Final amount: `₹1,000`

The program uses variables, strings, integers, floats, functions, parameters, return values, input, type conversion, comparison operators, conditional statements, and formatted output. It does not use a database, files, APIs, external libraries, or classes.