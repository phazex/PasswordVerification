f=open('passwordlog.txt' , 'w')

def lenCheck(password):
    if len(password) >= 8:
        return 1
    else:
        return 0
def passCheck(conpass , password):
    if (conpass==password):
        return 1
    else:
        return 0
def hasNumbers(password):
    test = any(char.isdigit() for char in password)
    if (test > 0):
        return 1
    else:
        return 0
def hasLower(password):
    test1 = any(c.islower() for c in password)
    if (test1 > 0):
        return 1
    else:
        return 0
def hasupper(password):
        test1 = any(c.isupper() for c in password)
        if (test1 > 0):
            return 1
        else:
            return 0

test=0


while test==0:
    password = input('Password:')
    conpass = input('Please Confirm Your Password:')

    if ( passCheck(password, conpass)==0):
        print("Passwords do not match, please check again.")
    if(lenCheck(password)==0):
        print('Please make password longer.')
    if (hasNumbers(password)==0):
        print('Please add a number.')
    if (hasupper(password)==0):
        print('Please add uppercase letter.')
    if (hasLower(password)==0):
        print('Please add a lowercase letter.')
    if(hasLower(password)==hasupper(password)==hasNumbers(password)==lenCheck(password)==passCheck(password, conpass)==1):
        print('Thanks for signing up.')
        f.write (password)
    else:
        test = 1
        print('There was a error please fix the parameters.')
    f.close()







