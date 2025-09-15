# Exp.No:29  
## Encapsulation

### AIM  
To write a Python program to create a class `Student` with the private members `name` and `age`, and add getter and setter methods to initialize and modify the `age` variable.

### ALGORITHM

1. **Start the Program.**
2. **Define the `Student` class.**
   - Inside the `Student` class, define the `__init__` method to initialize `name` and the private member `__age`.
3. **Define a getter method** `get_age` to return the value of the private member `__age`.
4. **Define a setter method** `set_age` to set a new value to the private member `__age`.
5. **Create an object `stud`** of the `Student` class with the name 'Jessa' and age 14.
6. **Print the name and the age** of `stud` using the getter method.
7. **Use the setter method** `set_age` to change the age of `stud` to 16.
8. **Print the name and the updated age** of `stud` using the getter method.
9. **End the program.**

### PROGRAM

```
class Student:
    def __init__(self, name, roll_no, age):
        self.name = name
        self.__roll_no = roll_no
        self.__age = age

   def show(self):
        print('Student Details:', self.name, self.__roll_no)

   
   def get_roll_no(self):
        return self.__roll_no


   def set_roll_no(self, number):
        if number > 50:
            print('Invalid roll no. Please set correct roll number')
        else:
            self.__roll_no = number
jessa = Student('Jessa', 10, 15)
jessa.show()
jessa.set_roll_no(52)
jessa.set_roll_no(25)
jessa.show()
```

### OUTPUT
![image](https://github.com/user-attachments/assets/b5125699-b8cd-46d6-ad12-3d23b982508a)

### RESULT

Thus the program to create class with private members and add getter and setter methods to initialize and modify the given variable has been implemented and executed successfully.


