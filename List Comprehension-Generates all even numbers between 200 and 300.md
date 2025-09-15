# 🧾 List Comprehension
## 🎯 AIM:
To Write a Python program to generate an Arithmetic Progression using list Comprehension with first number, difference and last number as input.
---

## 🧠 ALGORITHM:

1. **Start**
2.Define a Class: Create a class named Generate that will encapsulate the logic for generating the arithmetic progression.

3.Initialize the Class (__init__): In the constructor (__init__), accept three parameters: first (the starting number), d (the common difference), and last (the ending number). Store these values as instance attributes (self.first, self.d, self.last).

4.Define the Generator Method: Create a method within the class, named Ap_generate, which will perform the list generation.

5.Implement List Comprehension: Inside the Ap_generate method, use a list comprehension [i for i in range(self.first, self.last + 1, self.d)] to create the arithmetic progression. This will iterate from the first number to the last number (inclusive), with a step size of d.

6.Return the List: The Ap_generate method should return the newly created list containing the arithmetic progression. 
7. **Stop**

---

## 💻 PROGRAM:
```
class Generate:
    def __init__(self, first,d,last):
        self.first = first
        self.d = d
        self.last=last
    def Ap_generate(self):
        L=[i for i in range(self.first,self.last+1,self.d)]
        return L

f=int(input())
diff=int(input())
l=int(input())
Series = Generate(f,diff,l)
print('First Number', Series.first)
print('Difference', Series.d)
print('Last Number', Series.last)
print(Series.Ap_generate())
```

## OUTPUT:
<img width="1152" height="462" alt="image" src="https://github.com/user-attachments/assets/46c1d627-e472-4096-93ef-0a448c68176c" />


## RESULT:
Thus,the program is successfully created.
