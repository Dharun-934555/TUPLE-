                                              ##### TUPLE #####
                                          #### THIS IS FOR MY JUNIORS ####
                                        ### ALL THE BEST FOR USER FUTURE GOAL ###
INTRODUCTION :
     A tuple is a collection of ordered elements in Python.
        👉 It is similar to a list, but the difference is:
              * Tuple is immutable → once created, you cannot change, add, or remove its elements.
              * Tuples are written with round brackets ().
EXAMPLE : 
    my_tuple = (10, 20, 30, "Apple")
    print(my_tuple)    # OUTPUT : (10, 20, 30, 'Apple')
✨ TYPES OF TUPLE : 
           🚀 Empty Tuple
           🚀 Single-element Tuple
           🚀 Homogeneous Tuple
           🚀 Heterogeneous Tuple
           🚀 Nested Tuple
           🚀 Tuple with Repeated Elements
           
📘 Basic Tuples in Python : 

🍀 Empty Tuple :
          A tuple with no items.
          EXMAPLE : t = ()    
           
🍀 Single-element Tuple : 
          A tuple with only one item (must use a comma).
          EXAMPLE : t = (5,)

🍀Homogeneous Tuple : 
          All items are of the same type.
          EXAMPLE : t = (1, 2, 3, 4)

🍀Heterogeneous Tuple : 
          Items of different types.
          EXAMPLE : t = (1, "Apple", 3.5)

🍀Nested Tuple : 
          A tuple inside another tuple.
          EXAMPLE : t = (1, (2, 3), 4)

🍀Repeated Elements Tuple :
          A tuple with duplicate values.
          EXAMPLE : t = (2, 2, 3, 3, 3)  
EXERCISE 1 : 
     1. Create an empty tuple
     2. Create a tuple containing names of your sisters and your brothers (imaginary siblings are fine)
     3. Join brothers and sisters tuples and assign it to siblings
     4. How many siblings do you have?
     5. Modify the siblings tuple and add the name of your father and mother and assign it to family_members

EXERCISE 2 :
    1. Unpack siblings and parents from family_members
    2. Create fruits, vegetables and animal products tuples. Join the three tuples and assign it to a variable called                food_stuff_tp.
    3. Change the about food_stuff_tp  tuple to a food_stuff_lt list
    4. Slice out the middle item or items from the food_stuff_tp tuple or food_stuff_lt list.
    5. Slice out the first three items and the last three items from food_staff_lt list
    6. Delete the food_staff_tp tuple completely
    7. Check if an item exists in  tuple:

   - Check if 'Estonia' is a nordic country
   - Check if 'Iceland' is a nordic country

IMPLEMENTATION : 

# create empty tuple
   empty_tuple = ()
   print(empty_tuple)   #()
    
# using constructor
  empty_tuple = tuple()
  print(empty_tuple)  
    
# tpl with initial value
   tpl=("dharun","royal","sivan","preethi","aish","1213")
   print(tpl)  #'dharun','royal','sivan','preethi','aish','1213'
   print(len(tpl))
     
# positive index
  print(tpl[0])
    
# negative index
   print(tpl[-2])
   last=len(tpl)-1
   print(last)
   last_tpl=tpl[last]
   print(last_tpl)
   
# slicing positive tuple
   print(tpl[:4])
   print(tpl[4:6])
   print(tpl[:6:2])
   
# slicing negative tuple
  print(tpl[-4:-1])
  print(tpl[-6:-1:2])
  
# tuple change into list
  my_list=list(tpl)
  print(my_list[0])
  tpl=tuple(my_list)
  print(tpl)
# check an item in a tuple
  tpl=("dharun","royal","sivan","preethi","aish","1213")
  print("logana"in tpl)
  
# joining tuple
  tpl1=("logana","1234","3456")
  tpl2=tpl+tpl1
  print(tpl2)
  
# deleting tuple
  tpl1=("logana","1234","3456")
  del tpl1

# EXERCISE : 

  empty_tpl=()
  print(empty_tpl)
  name=("preethi","gayathri","divya","sahana")
  name1=("dharaneesh","giri","vivith","hari")
  siblings=name+name1
  print(siblings)
  print(len(siblings))
  family_member=siblings
  print(family_member)
  family_member1=("saravanan","karthigai selvi")
  family=family_member+family_member1
  print(family)
  fam=(family_member,family_member1)
  all_sibling,all_parents=fam
  print("siblings:",all_sibling)
  print("parents:",all_parents)

# other tuple : 

  fruits=("apple","orange","grapes")
  vegetables=("carrot","tomato","potato")
  animals=("dog","cat","lion")
  food_stuff_tp=fruits+vegetables+animals
  print(food_stuff_tp)
  food_stuff_lt=list(food_stuff_tp)
  print(food_stuff_lt)
  l=len(food_stuff_lt)
  print(l)
  if l %2!=0:
      middle_items=food_stuff_lt[l//2-1 : l//2+1]
  else:
      middle_items=[food_stuff_lt[l//2]]
  print(middle_items)
  print(food_stuff_lt[:3],food_stuff_lt[-3:])
  del food_stuff_tp
  try:
      print("dog"in food_stuff_tp)
  except:
      print("you cannot access the food_stuff_tp,because it already deleted")
       
      
