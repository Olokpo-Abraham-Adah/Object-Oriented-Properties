class Account:
    def __init__(self):
        self.balance = 10000
        self.interest_rate = 5
        self.__id_number = "D6137898"
        print("starting balance is", self.balance)

    def deposit(self, amount):
        self.balance = amount + self.balance
        print("new balance is:", self.balance)

    def withdraw(self, amount):
        self.balance = self.balance - amount
        print("new balance is", self.balance)

        from account import Account


class currentAccount(Account):
    def __init__(self):
        Account.__init__(self)


currentAccount = currentAccount()
currentAccount.deposit(5000)
currentAccount.withdraw(1500)

from account import Account


class SavingsAccount(Account):
    def __init__(self):
        Account.__init__(self)

    def withdrawal(self, amount):
        if amount < 2000:
            supper() . withdraw(amount)
        else:
            print("you can not withdraw above your limit")


SavingsAccount = SavingsAccount()
SavingsAccount.withdraw(1000)
