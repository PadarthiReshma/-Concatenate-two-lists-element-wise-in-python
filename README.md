# -Concatenate-two-lists-element-wise-in-python

# Apporach-1
# Python3 code to demonstrate 
# interlist element concatenation
# using list comprehension + zip()
                       
# initializing lists 
test_list1 = ["Geeksfor", "i", "be"]
test_list2 = ['Geeks', 's', 'st']

# printing original lists
print ("The original list 1 is : " + str(test_list1))
print ("The original list 2 is : " + str(test_list2))

# using list comprehension + zip()
# interlist element concatenation
res = [i + j for i, j in zip(test_list1, test_list2)]

# printing result 
print ("The list after element concatenation is : " + str(res))

# Apporach-2

# Initialize the lists
list1 = ["Hello", "Hi", "Good morning"]
list2 = ["world", "there", "all"]

# Use reduce() to concatenate the elements
from functools import reduce
result = reduce(lambda res, l: res + [l[0] + " " + l[1]], zip(list1, list2), [])

print(result)                                                                                                                                                                                                   


# Apporach-3
test_list1 = ["Geeksfor", "i", "be"]
test_list2 = ['Geeks', 's', 'st']
# printing original lists
print ("The original list 1 is : " + str(test_list1))
print ("The original list 2 is : " + str(test_list2))
res = []
for i in range(len(test_list1)):
	res.append(test_list1[i]+test_list2[i])
print("The list after element concatenation is : " + str(res))
#This code is contributed by Jyothi pinjala.


                                                                                                                                                                                                                                                                                                                                                                                                 
                                                                                                                                                                                                                                                                                                                                                                                                           
