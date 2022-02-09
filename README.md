# Word-count
## AIM:
To write a python program for getting the word count from a text.
## EQUIPEMENT'S REQUIRED: 
PC
Anaconda - Python 3.7
## ALGORITHM: 
### Step 1:
Assign a variable for value zero
### Step 2: 
 open then required file by using the function "with"
### Step 3: 
Then use the for loop for assigning the i value in the file
### Step 4:  
using split function to split the words
### Step 5: 
Finding the length of the words by using len() function
### Step 6: 
Calling the function and printing the number of words.
## PROGRAM:
```
#text.txt
with open("mytext.txt",'w')as fp:
  fp.write("名はうちはサスケ")
  fp.write("\n一族の復興とある男を必ず殺すことだ。")
  fp.write("\nお前ら忍者なめてんのか\n")
def wordcount(filename):
  count = 0
  with open(filename,"r") as f1:
    data=f1.readlines()
    for line in data:
      word=line.split()
      for i in word:
          count += 1
  print("The word count is", count)
filename=input("Enter filename:")
wordcount(filename)
```
### OUTPUT:
![image](https://user-images.githubusercontent.com/94810884/153128362-9c884d48-1629-4e1f-9408-d496181517fc.png)

![image](https://user-images.githubusercontent.com/94810884/153128396-47e903ff-f0d3-4cc1-bddb-37f78c8d51ac.png)



## RESULT:
Thus the program is written to find the word count from a text.
