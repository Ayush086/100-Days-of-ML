# Today's Learnings
*Explored some rarely used variables handling like mixed variables, time and date data handling.*

## Mixed Variables Handling
First of all let's try to understand,  
 **what is mixed variable ?**  
Mixed Data = Numerical Data + Categorical Data   
eg.   
![Screenshot 2024-10-31 000828](https://github.com/user-attachments/assets/f5277fd7-173f-4e5b-913c-af6c4faf14f8)  

which can then divided into 2 parts: Category, Seat Number  
![Screenshot 2024-10-31 000836](https://github.com/user-attachments/assets/8ee67d3b-cba9-4bed-ae7f-a6933156c7cb)


**It's recommended that whenever you tackle with mixed data always try to divide it into 2 columns (numerical, categorical)**  
After division it will be more feasible for model to understand data.  

## Date and Time Variables Handling
Usually date is complex to handle there are various ways in which it's represented and it showcase many hidden information. 
If you are given a random date you can determine the month, week, quarter, year, etc.  
Similarly for time it contains  days, hours, mins, etc.

It's not very hard to handle them.
Just remember that, In pandas date/time are treated as string/object.
So before making any changes to change them into **datetime** datatype.

***pd.to_datetime()*** is used for the conversion in pandas. After the conversion you can perform required operations.  


***All implementation performed during learning are stored in python notebooks which are attached within this folder***

