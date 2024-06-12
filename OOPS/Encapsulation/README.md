### Encapsulation

**Encapsulation** is one of the fundamental principles of object-oriented programming (OOP). It refers to the bundling of data (attributes) and methods (functions) that operate on that data into a single unit, known as a class. Encapsulation also restricts direct access to some of an object's components, which can prevent the accidental modification of data.

In Python, encapsulation is achieved through access modifiers. These modifiers determine the accessibility of the data members (attributes) and member functions (methods) of a class. Here are the main types of access modifiers:

1. **Public**: Members are accessible from anywhere.
2. **Protected**: Members are accessible within the class and its subclasses.
3. **Private**: Members are accessible only within the class itself.

Encapsulation helps to achieve the following:
- **Data Hiding**: By restricting access to certain members of an object, we can hide its internal state and protect it from unwanted modification.
- **Modularity**: Encapsulation enables the creation of modular, self-contained units of functionality.
- **Maintenance**: It makes maintaining and updating the code easier since changes to encapsulated code are less likely to affect other parts of the program.


### Example

```python
class Account:
    def __init__(self, owner, balance):
        self.owner = owner  # Public attribute
        self.__balance = balance  # Private attribute

    @property
    def balance(self):
        return self.__balance

    @balance.setter
    def balance(self, amount):
        if amount >= 0:
            self.__balance = amount
        else:
            print("Invalid amount! Balance cannot be negative.")

    def deposit(self, amount):
        if amount > 0:
            self.__balance += amount
            print(f"Deposited {amount}. New balance is {self.__balance}.")
        else:
            print("Invalid deposit amount!")

    def withdraw(self, amount):
        if 0 < amount <= self.__balance:
            self

.__balance -= amount
            print(f"Withdrew {amount}. New balance is {self.__balance}.")
        else:
            print("Invalid withdrawal amount!")

# Create an account object
account = Account("John", 1000)
print(account.owner)  # Accessing public attribute
print(account.balance)  # Accessing private attribute via getter

account.deposit(500)
account.withdraw(200)
print(account.balance)  # Accessing updated balance

account.balance = 1500  # Using setter to update balance
print(account.balance)

account.balance = -500  # Trying to set an invalid balance
```

Output:
```
John
1000
Deposited 500. New balance is 1500.
Withdrew 200. New balance is 1300.
1300
1500
Invalid amount! Balance cannot be negative.
```

By understanding and using access modifiers and encapsulation, you can design more robust and secure classes in Python. If you have any questions or need further clarification, feel free to ask!
