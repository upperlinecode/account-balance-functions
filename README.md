# Account Balance Calculator Lab

![counting money](https://media.giphy.com/media/13LIwnzH6PFt0A/giphy.gif "Counting Money")

Whether you have a (grown-up) bank account or you're still using a piggy bank, it's always important to know how much money you have... so you can know how much money you can spend!

In general, we can write a set of instructions (an algorithm) to help us save and spend our money more responsibly. In this lab, you'll be using python methods to create the functions that will be used in a simple Account Balance Calculator.

## Instructions

1) Create a notification method called `getBalance()` that takes an input of the `balance` and returns a message to the user.

```python
def getBalance(balance):
	# your code here
```

> If your method throws an error, try googling the error to find a solution.

**Example:** When I run `getBalance(300)`, it should return **You have $300 in your account**.

```python
print(getBalance(300))
# You now have $300 in your account.

print(getBalance(615))
# You now have $615 in your account.
```

2) Create a deposit method called `makeDeposit()` that takes two inputs - the current `balance` and the deposit `amount` and returns the resulting account balance.

```python
def makeDeposit(balance, amount):
	# your code here
```

**Example:** When I run `makeDeposit(500, 32)`, it should return **532**.

```python
print(makeDeposit(500, 32))
# 532
```

3) Update your `makeDeposit()` method using your `getBalance()` method so it returns a message instead of just a number.

```python
print(makeDeposit(500, 32))
# You now have $532 in your account.
```

4) Create a `makeWithdrawal()` method that takes two inputs - the current `balance` and the withdrawal `amount` and returns the resulting account balance.

```python
def makeWithdrawal(balance, amount):
	# your code here
```

**Example:** When I run `makeWithdrawal(200, 73)`, it should return **127**.

```python
print(makeWithdrawal(200, 73))
# 127
```

5) Update your `makeWithdrawal()` method using your `getBalance()` method so it returns a message instead of just a number.

```python
print(makeWithdrawal(200, 73))
# You now have $127 in your account.
```

6) Create a method `overdraft()` that takes an account `balance` as an input and returns a notice to a user if their account is overdrawn (negative).

```python
def overdraft(balance):
	# your code here
```

**Example:** When I run `overdraft(-25)`, it should return **Your account is overdrawn!**, but if I run `overdraft(30)`, it should not return a message.

```python
print(overdraft(-25))
# Your account is overdrawn!

print(overdraft(30))
#
```

7) Include the `overdraft()` method in your `makeWithdrawal()` method so `makeWithdrawal()` returns a message if the result of the withdrawal is a negative account balance.

```python
print(makeWithdrawal(20, 35))
# Your account is overdrawn!
```

8) Modify your `overdraft()` method to indicate to a user by how much their account is overdrawn.

```python
print(overdraft(-12))
# Your account is $12 overdrawn!
```

> Note: Be sure to account for changing the numerical value from -12 to positive 12.

9) Some banks charge a fee whenever a user overdraws their account. Update your `makeWithdrawal()` method to assess a $25 fee whenever an account is overdrawn.

**Example:** When I run `makeWithdrawal(10, 30)`, it should return **Your account is $45 overdrawn!** because the withdrawal results in a -$20 balance but the additional $25 fee results in a -$45 balance.

```python
print(makeWithdrawal(10, 30))
# Your account is $45 overdrawn!
```
