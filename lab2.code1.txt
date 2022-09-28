# -*- coding: utf-8 -*-
"""
Created on Wed Sep 28 10:55:37 2022

@author: nshut
"""

def gcd(a,b):
    
    if (a == 0):
        return b
    return gcd(b % a, a)

def phi(n):
    
    result = 1
    for i in range(2, n):
        if (gcd(i, n)==1):
            result += 1
    return result

n = int(input("Enter number here: "))

print("phi(",n,") = " ,
      phi(n), sep = "" )


#for n in range(1,11):
#    print("phi(",n,") = " ,
#          phi(n), sep = "" )

#n = int(input("Enter value here: "))

#range = [1,n-1]

#euFunction = []

#for number in range:
#    if number 