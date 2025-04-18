# SELECTION SORT AND INSERTION SORT 

## AIM :

To write a program to perform selection sort and insertion sort using python programming.

## EQUIPMENTS REQUIRED :

-	Hardware – PCs  
-	Anaconda – Python 3.7 Installation / Moodle-Code Runner

## ALGORITHIM :

## SELECTION SORT ALGORITHIM :

1.	Set the first unsorted element as the minimum
2.	For each of the unsorted elements, check if the element < current minimum.
3.	If yes, set the element as the new minimum.
4.	Swap minimum with first unsorted position.
5.	Repeat the steps 2 and 3 for all the elements in the array.

## INSERTION SORT ALGORITHIM :

1.	Set the first element as sorted element j.
2.	For each unsorted element X, check if current sorted element j >X.
3.	If yes, move sorted element to the right by 1.
4.	Break the loop and insert X.
5.	Repeat the steps 2 to 4 for sorting all the elements in the array.

## PROGRAM :

###  SELECTION SORT :
```python
Developed by: MIDHUN AZHAHU RAJA P
RegisterNumber: 22008311

def selection_sort(nums):
    for i in range(len(nums)):
        lowest_value_index=i
        for j in range(i+1,len(nums)):
            if nums[j]<nums[lowest_value_index]:
                lowest_value_index=j
        nums[i],nums[lowest_value_index]=nums[lowest_value_index],nums[i]
list_of_nums=eval(input())
selection_sort(list_of_nums)
print(list_of_nums)


```

### INSERTION SORT :

```PYTHON
Developed by: MIDHUN AZHAHU RAJA P
RegisterNumber: 22008311

def insertion_sort(nums):
    for i in range(1,len(nums)):
        item_to_insert=nums[i]
        j=i-1
        while j>=0 and nums[j]>item_to_insert:
            nums[j+1]=nums[j]
            j-=1
        nums[j+1]=item_to_insert
list_of_nums=eval(input())
insertion_sort(list_of_nums)
print(list_of_nums)
```
## INPUT :

### INPUT FOR SELECTION SORT :
![image](https://user-images.githubusercontent.com/118054670/213933037-8494437f-4176-49fa-b5ce-a760439d1d79.png)


### INPUT FOR INSERTION SORT :

![image](https://user-images.githubusercontent.com/118054670/213933018-4c0b0ba7-bb9e-4bb0-b312-5fe07bbd6806.png)

## OUTPUT :

### OUTPUT FOR SELECTION SORT :

![image](https://user-images.githubusercontent.com/118054670/213932415-c3811b31-724d-4e3a-a8d6-ef1565f7220f.png)

### OUTPUT FOR INSERTION SORT :

![image](https://user-images.githubusercontent.com/118054670/213932783-c860749b-93b9-4fda-a5b5-5cc507c63563.png)

## RESULT :

Thus the program is written to perform selection sort and insertion sort using python programming.
