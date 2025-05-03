# Aim:
To create a Flowchart in UiPath using Repeat, While, and Do While loops to perform simple counting or message display tasks.

## Software Required:
```
1.UiPath Studio (2021 or later version recommended)
2.Windows Operating System
```
## PROCEDURE:

## 1. Open UiPath Studio:
     Launch UiPath Studio on your system.
## 2. Create a New Project:
            a.Click on "Process".
            b.Give the project a name (e.g., LoopFlowchartDemo).
            c.Click Create.

## 3. Replace Default Sequence with Flowchart:
           a.In Main.xaml, delete the default Sequence activity.
           b.From the Activities panel, drag and drop a Flowchart into the Designer panel.

## A. Repeat (For Each) Loop Section:
         a.Add a Flow Step and rename it as "Start - Repeat".
         b.Add an Assign activity:
            numbers = {1, 2, 3}
            (Create variable numbers of type Integer[] or Array of Int32)
         c.Add a For Each activity:
            *TypeArgument: Int32
            *Values: numbers
            *Inside the For Each, add a Message Box:
               Message: "Repeat: Number is " + item.ToString

## B.While Loop Section:
     a.Add another Flow Step and rename it as "Start - While".
     b.Declare variables:
        countWhile = 1 (Type: Int32)
        max = 3 (Type: Int32)
    c.Add a While activity:
       Condition: countWhile <= max
    d.Inside the While:
        *Add a Message Box:
           Message: "While: Count is " + countWhile.ToString
        *Add an Assign activity:
           countWhile = countWhile + 1

## C. Do While Loop Section:
   a.Add a third Flow Step and rename it as "Start - DoWhile".
   b.Declare variable:
      countDo = 1 (Type: Int32)
   c.Add a Do While activity:
      *Condition: countDo <= 3
      *Inside the Do While:
        Add a Message Box: 
           Message: "DoWhile: Count is " + countDo.ToString
        Add an Assign activity:countDo = countDo + 1

## Workflow:
![Screenshot 2025-05-03 124956](https://github.com/user-attachments/assets/f4229115-9f14-4ef3-95fa-6c128f8e24e1)
![Screenshot 2025-05-03 125327](https://github.com/user-attachments/assets/0fea9600-e092-48e8-9aef-cba8f6a44c7d
![Screenshot 2025-05-03 131951](https://github.com/user-attachments/assets/10407ffe-fec1-4d38-9d7b-5a4b17db484b)



## OUTPUT:
![image](https://github.com/user-attachments/assets/14175f18-0b5a-48b3-a11d-92a61ac6d15a)
![image](https://github.com/user-attachments/assets/c7950c53-1c20-41a3-9e05-bcabd91ab56d)
![image](https://github.com/user-attachments/assets/66aeea28-46e9-45c5-bbf5-d508a0436507)

## Result:
```
When you run the Flowchart:
   1.You will see "Repeat: Number is 1, 2, 3"
   2.Then "While: Count is 1, 2, 3"
   3.Then "DoWhile: Count is 1, 2, 3"
```




