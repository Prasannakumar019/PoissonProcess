## EX NO:06
## DATE:8.6.22
# <p align="center">Poisson Process

# Aim : 
To find the probability of that  (i) exactly 4 customers arrive (ii) more than 4 customers arrive (iii) fewer than 4 customers in 2 minute  arrival. Given that the customers arrive at a bank according to a Poisson process with mean rate of 3 per minute  during a time interval of 2 min. 


# Software required :  

Python

# Theory:

The Poisson process is one of the most widely-used counting processes. It is usually used in scenarios where we are counting the occurrences of certain events that appear to happen at a certain rate, but completely at random (without a certain structure). For example, suppose that from historical data, we know that earthquakes occur in a certain area with a rate of 2 per month. Other than this information, the timings of earthquakes seem to be completely random. Thus, we conclude that the Poisson process might be a good model for earthquakes. In practice, the Poisson process or its extensions have been used to model.

1. The number of car accidents at a site or in an area
2. The location of users in a wireless network
3. The requests for individual documents on a web server

 
# Procedure :

![image](https://user-images.githubusercontent.com/104613195/171325180-eaf80506-545c-4f35-878a-1e95aa0e81e3.png)



# Program :
```python
Developed by: Prasannakumar M
Registration number:212220230035
import numpy as np
import math

l=3
t=2

def p(x):
    return round(math.exp(-l*t)*((l*t)*x)/math.factorial(x),2)

print("probability that exactly 4 customers arrive",p(4))

n=1-(p(0)+p(1)+p(2)+p(3)+p(4))
print("probability that more than 4 customers arrive",n)

m=p(0)+p(1)+p(2)+p(3)
print(" rate of 3 per minute during a time interval of 2 min.",m)
 ```

# Output : 
 ![11](https://user-images.githubusercontent.com/75235090/172536213-8e9a4853-c5e3-4d5d-8df7-89941ff5ebf6.png)
# Result :
Thus, the program to find the probability of the given conditions using Poisson process is implemented.
