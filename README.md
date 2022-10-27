# Day5-Lab2-Dictionary

Build a phone book program that receives the phone number, and returns the name of the owner. 
You can follow the table below:

| Name    | Number      |
| -------- | ---------- |
| Amal     | 1111111111 |
| Mohammed | 2222222222 |
| Khadijah | 3333333333 |
| Abdullah  | 4444444444 |
| Rawan    | 5555555555 |
| Faisal   | 6666666666 |
| Layla    | 7777777777 |


- If the number exists, print the owner. Otherwise, print "Sorry, the number is not found".
- If the number is less or more than 10 numbers, print "This is invalid number".
- If the number contains letters or symbols, print "This is invalid number".






entry = input("Enter a phone number:")

mydict = {'Amal': '1111111111',
          'Mohammed': '2222222222',
          'Khadijah': '3333333333',
          'Abdullah' : '4444444444',
          'Rawan' : '5555555555',
          'Faisal' : '6666666666',
          'Layla' : '7777777777'}


for key, value in mydict.items():
    
    x = len(entry)
    if (10>x<10):
        print("This is invalid number!")
        break
   

    if mydict[key] == entry:
        print("The owner is:   " + key)
        break
    
else:
    print("Sorry, the number is not found!")
    
   
    
