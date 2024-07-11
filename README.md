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

       
