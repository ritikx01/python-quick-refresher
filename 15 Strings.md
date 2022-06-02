String is always written between double quotes (or single).
Ex: "for", "Text".

**This part is a bit lengthy but it covers almost all the string manipulation techniques**

## String manipulation
### 1. String indexing
1. String indexing (Positive)
We can index a string and access the character we want to
Ex-
```python
name = "Ritik"
print(name[1])
a										#Ouput
```
- Python starts counting indexes from 0, hence "a" is displayed at the first place.
2. String Indexing (Negative)
```python
text = "Some Random text"
print(text[-1])
t										#Output
print(text[-2])
x										#Output
```
### 2. String multiplication
```python
"example" *3 
exampleexampleexample					#Output
```
### 3. String slicing (Access part of a string )
```python
colour = "Orange"
print(colour[1:4])
ran										#Output #Index from 1 to 4(EXCLUDED) is printed
```
- We can leave first or last index value empty in square bracket while slicing. Python would assume:
	1. Start of string - If start value is empty.
	2. End of string - If end valuse is empty.
Ex- 
```python
colour = "Orange"
print(colour[:4])
Oran									#Output
print(colour[3:])
nge										#Output
```
### 4. Editing a string
A string can not be edited in a variable but rather edited and assigned to a new variable.
```python
message = "A kong string with a silly typo"
new_message = message[0:2] + "l" + message[3:]
print(new_message)
A long string with a silly typo			#Output
```
### 5. Search for a character in string
```python
pets = "Cats & Dogs"
print(pets.index("&"))
5										#Output
```
- Here we have used `.index` which is a **Method**. It is a function associated with a specific class.
```python
pets = "Cats & Dogs"
print(pets.index("C"))
0										#Output
print(pets.index("Dog"))
7										#Ouput #Returns the index of the substring
print(pets.index("s"))
3										#Output # return the index of first occurence of the character.
```
### 6. Check if a substring is present in a string
```python
pets = "Cats & Dogs"
print("Dragon" in pets)
False									#Output
print("Cats" in pets)
True									#Output
```
### 7. Transformation / Formatting
```python
print("Mountains".upper())
MOUNTAINS
print("Mountains".lower())
mountains
```
Ex:
```python
answer = 'YES'
if answer.lower() == "yes":
	print("USer typed Yes")
	
User typed Yes							#Output
```
### 8. Remove surrounding (space/tab/newline character)
This strip METHOD doesn't work for white spaces in between of words, to remove space from in between words, use replace method (below).
```python
word = "  yes  "
print(word.strip())
"yes"									#Output
print(word.lstrip())					#Remove spaces from left side of the word
"yes  "
print(word.rstrip())
"  yes"
```
### 9. Count a character in a string(no. of occurance) 
```python
string = "The number of times e occurs in this string"
print(string.count("e"))
4										# Output
```
### 10. Check what is at the end of the string
```python
text = "I have a dog"
print(text.endswith("dog"))
True									# Output
print(text.endswith("og"))
True									# Output
```
### 11. Check if a string is made with just numbers
```python
print("A string".isnumeric())
False									#Output
print("12345".isnumeric())				
True									#Output
```
### 12. Convert a numeric string to numbers
```python
num = int('2343')
print(type(num))
<class 'int'>							#Output
```
### 13. Join a list by anything
```python
" ".join(["The", "phrase", "is", "joined"])
The phrase is joined					#Output
"...".join(["The", "phrase", "is", "joined"])
The...phrase...is...joined				#Output
"a".join("rttt ")
ratatata								#Output		#Notice the space in the end in "rttt ". This is must to append 'a' at the end.
```
### 14. Split a string into list
```python
"Split this string".split()
['Split', 'this', 'string']
```