# syseng
Assignment for the course System Engineering will be added here.

# Lesson 1 Open Addressing


# Lesson 2 B+tree leaf insert 11OCT
The following code is added to line 70 and 71 in ./btree/bptree.cc
	
    leaf->key[i] = key;
    leaf->chi[i] = (NODE *)data;

If the key input is larger than value in leaf, it will go through step 1 (the for loop in line 65 to 66), in which the highest value in leaf that is less than or equal to key input is found.  After that, the input key and the pointer will be inserted just after previous highest value. 

For example, if the input pattern is first entered as 1 then followed by 2 and 3, the result will be  
[1]  
[1 2]  
[1 2 3]  

Similarly, when the input pattern is entered as 3 followed by 2 and 1, the result will be  
[3]  
[2 3]  
[1 2 3]  

![Execution Screenshoot] (https://gyazo.com/5c8ebef5c4a796c50f865e07c01af445)  
# Lesson 3 18OCT

