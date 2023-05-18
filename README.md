Method1:-
Str="SamChandu"
lower=0
upper=0
for i in Str:
      if(i.islower()):
            lower+=1
      else:
            upper+=1
print("The number of lowercase characters is:",lower)
print("The number of uppercase characters is:",upper)
Method2:-

def upperlower(string):
    upper = 0
    lower = 0
  for i in range(len(string)):
          # For lower letters
        if (ord(string[i]) >= 97 and
            ord(string[i]) <= 122):
            lower += 1
 # For upper letters
        elif (ord(string[i]) >= 65 and
            ord(string[i]) <= 90):
            upper += 1
 print('Lower case characters = %s' %lower,
        'Upper case characters = %s' %upper)
 
# Driver Code
string = 'SanapathiSaiSameeraGolluRamchandrao'
upperlower(string)
Method3:-
import operator as op
Str = "SanapathiSaiSameeraGolluRamchandrao"
lower = "abcdefghijklmnopqrstuvwxyz"
low = 0
upp = 0
for i in Str:
    if op.countOf(lower, i) > 0:
        low += 1
    else:
        upp += 1
print("The number of lowercase characters is:", low)
print("The number of uppercase characters is:", upp)
