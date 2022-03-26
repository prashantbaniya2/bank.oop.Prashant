# bank.oop.Prashant
#oop by prashant 
class Bank:
    __bank_name = 'Blue Bank Pvt. Ltd. '
    __interest_rate = 8
    def __init__(self,first_name,last_name,address):
        self.__first_name = first_name
        self.__last_name = last_name
        self.__address = address
        self.__balance = 0
#to print the current balance of user
    def check_balance(self):
        print(f'your current balance is {self.__balance}')
        
    def password(self,pin):
        password = pin
        print(f'your pin is{pin}')
    
    
    def deposit_balance(self,deposit_amount,password):
        if deposit_amount < 0:
            print('invalid amount')
            
           
        
        else:
            password == pin
            self.__balance = self.__balance + deposit_amount
            print(f'Updated balance is {self.__balance}')
    
    
    def withdraw_balance(self,withdraw_amount):
        if withdraw_amount > self.__balance:
            print(f'invalid amount::please withdraw amount upto{self.__balance}')
        else:
            password == pin
            self.__balance == self.__balance - withdraw_amount
            

    def set_new_pin(self,new_pin):
        user.password = new_pin
        Bank.get_set_new_pin
            
    @classmethod
    def get_bank_name(cls):
        return Bank.__bank_name
    
    @classmethod
    def get_interest_rate(cls):
        print(f'Your interest rate is{Bank.__interest_rate}')
    
    @classmethod
    def set_interest_rate(cls,new_rate):
        Bank.__interest_rate = new_rate
        Bank.get_interest_rate()
    
    @staticmethod
    def happy_holiday():
        print('holi from chait 2 to 5')
        print('dashain holiday from falgun 2 to 14')
        print('tihar holiday from flagun 26 to 30')
        print('chaat holiday from magh 4 to 7' )
    

    
           
    
while True:
    print('*'*150)
    print(f'welcome to the  {Bank.get_bank_name()}')

    choice = input('enter 1 to open account. \nenter 2 to check balance. \n enter to 3 set pin for your account \nenter to 4 deposit amount. \nenter 5 to withdraw balance. \n enter 6 to know interest. \nenter 7 to change interest rate. \nenter 8 to print holidays , \nenter 9 to change your change your Pin' )
    
    if choice == '1':
        fn = input('enter your first name : ')
        ln = input('enter your last name:   ')
        addr= input('enter your adress:     ')
        user=Bank(first_name = fn,last_name = ln,address = addr)
        print('congratulations and celebration::Welcome to the Blue Family')
        
    elif choice == '2':
        user.check_balance()
        
        
    elif choice == '3':
         pin = int(input('enter to set pin'))
         user.password(pin)
        
        
    
    elif choice == '4' :
        deposit_amount = int(input('Enter deposit amount '))
        password = input('enter your pin ')
        user.deposit_balance(deposit_amount,password)
        
        
    elif choice == '5':
         withdraw_amount = int(input('enter amount to withdraw'))
         pin = input('enter your pin')
         user.withdraw_balance(withdraw_amount)

    elif choice == '6':
        Bank.get_interest_rate()
    
    
    elif choice == '7':
        print('!!!!!!!!!!!!!!!!!Beta/Beti Nagarum!!!!!!!!!!!!!!!')
        print('do not change the interest rate')
        choose = int(input('Enter 0 to exist \nEnter 1 to change interest rate' ))
        
        if choose == 0:
            pass
        
        elif choose == 1:
            new_rate = int(input('Enter new rate to apply '))
            Bank.set_interest_rate(new_rate)
            
    elif choice == '8':
        Bank.happy_holiday()
        
    elif choice == '9':
         print('!!!!!!!!!!!!!!!!!{{{Beta/Beti Nagarum}}}}!!!!!!!!!!!!!!!')
         check = int(input('Enter 1 to exist \nEnter 2 to change pin' ))
        
        if check == 1 :
            pass
        elif check == 2 :
            new_pin = input('enter new pin')
            Bank.set_new_pin(new_pin)
            
