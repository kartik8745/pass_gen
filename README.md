# pass_gen

import string 
import random
if __name__=="__main__":
  s1=string.ascii_lowercase
  s2=string.ascii_uppercase
  s3=string.digits
  s4=string.punctuation
  
  k=int(input("Enter the length off pass u wont: "))
  s=[]
  s.extend(list(s1))
  s.extend(list(s2))
  s.extend(list(s3))
  s.extend(list(s4))
  
  random.shuffle(s)

  print("Your Password is:  ",("".join(s[0:k])))
 
