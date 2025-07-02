#add
def add(num1 ,num2) :
  return (num1 + num2)
#subtract
def subtract(num1 , num2):
    return (num1 - num2)
#multiply
def multiply(num1 , num2):
    return (num1 * num2)
#divide
def divide(num1 , num2):
    return (num1 / num2)
#exponent
def exponent(num1,num2):
    return (num1 ** num2)
#square root
def square_root(num1 ,num2):
    return (num1 ** 0.5)
#cube root
def cube_root(num1 ,num2):
    return (num1 ** (1/3))
#circle_area
def circle_area(pi,r):
    return (pi*r**2)
#circle_perimeter
def circle_perimeter(pi,r):
    return (pi*2*r)   
#log
import math as m

try :
    
    print ("if you want to add enter (+) subtract enter (-) multiply enter (*) divide enter (/) exponent enter (^) square root enter (sqrt) cube root enter (cbrt) circle area enter (circle area) circle perimeter enter (circle perimeter) log10 enter (log10) log2 enter (log2) in opiration slot")   
    
    n1=float(input('enter your first number/radius for circle  : '))
    op=input('enter your opiration  :')
    n2=float(input('enter your second number/any number if you want to calculate a circle or root : '))   
    pi=22/7
   

    
    
except ValueError :
    print ("invalid input")

if op=='+':
    print ('result : ' , add (n1,n2))
    
elif op=='-':
    print ('result : ' , subtract (n1,n2)) 
    
elif op=='*':
    print ("result : " , multiply (n1,n2)) 
    
elif op=='/':
    print ('result : ' , divide (n1,n2))
    
elif op=='^':
    print ('result : ' , exponent (n1,n2))    

elif op=='sqrt':
    print ('result : ' , square_root (n1,n2))
    
elif op=='cbrt':
    print ("result : " , cube_root (n1,n2))

elif op=='circle area':
    print ("result : " , circle_area (pi,n1))

elif op=='circle perimeter':
    print ("result : " , circle_perimeter (pi,n1))

elif op=='log10':
    print (m.log10(n1))

elif op=='log2':
    print (m.log2(n1))
    
else:
    print (' invalid opiration')
