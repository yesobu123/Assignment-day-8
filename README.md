Assignment 1:                                                                                                                                    
 #Program to display the Fibonacci sequence up to n-th term                                                                                                           
nterms = int(input("How many terms? "))
#first two terms                                                                                                                                         
n1, n2 = 0, 1                                                                                                                                                        
count = 0                                                                                                                                                          
 #check if the number of terms is valid                                                                                                                          
if nterms <= 0:                                                                                                                                                              
   print("Please enter a positive integer")                                                                        
elif nterms == 1:                                                                                                                                       
   print("Fibonacci sequence upto",nterms,":")                                                                                                                          
   print(n1)                                                                                                                                                          
else:                                                                                                                                                                      
   print("Fibonacci sequence:")                                                                                                                                    
   while count < nterms:                                                                                                                                   
       print(n1)                                                                                                                                                          
       nth = n1 + n2                                                                                                                                          
       # update values                                                                                                                                       
       n1 = n2                                                                                                                                     
       n2 = nth                                                                                                                                                 
       count += 1                                                                                                                                                
                                                                                                                                                                       
        >>> How many terms? 7                                                                                                                               
Fibonacci sequence:                                                                                                                  
0                                                                                                                                  
1                                                                                                                                                                 
1 
2                                                                                                                                                
3                                                                                                                                              
5                                                                                                                                        
8                                                                                                  
>>>                   


Assignment 2:.                                                                                                                                                                   
def gen_arm():                                                                                                                                   
 for num in range(0, 1000):                                                                                                                              
    order = len(str(num))                                                                                                                                                              sum = 0                                                                                                                                                 
	  temp = num                                                                                                                                                            
	  while temp > 0:                                                                                                                                                       
	    digit = temp % 10                                                                                                                              
	    if order == 1:                                                                                                                                        
       order = 0                                                                          
      sum += digit ** order	                                                                                                                     
	    temp //= 10                                                                                                                                                       
	  if num == sum:                                                                                                                                              
	    yield num                                                                                                                                          
    # order of number                                                                                                                                         
    values = gen_arm()                                                                                                                                                   
for i in values:                                                                                                                                                     
	print(i)                                                                                                                                                                   

O/P:                                         
0                     
1                          
153                                                     
370                           
371                                         
407                            

