#bisection method of f(x)=2-e^x interval [0,1]
def f(x):
    return 2-np.exp(x)

n=0
a=0
b=1
err=1
root=(a+b)/2
err=abs((a-b)/2)
while err>0.001:
    c=(a+b)/2
    testb=f(c)*f(b)
    testa=f(c)*f(a)
    if testb<0:
        a=c
        root=(a+b)/2
        err=abs((a-b)/2)
    elif testa<0:
        b=c
        root=(a+b)/2
        err=abs((a-b)/2)
    else:
        print('error')
        break
    n=n+1
    print(n,'    ',a,'    ',b,'    ',err)
print('final=',root)   

#newton method
def f(x):
    return x-0.9*np.sin(x)-np.pi/2
def f1(x):
    return 1-0.9*np.cos(x)

n=0
x=2
dif=1
while dif>0.001:
    print(n,'   ',x)
    a=x-f(x)/f1(x)
    dif=abs(a-x)
    x=a
    n=n+1

#secant method
def f(x):
    return 2-np.exp(x)

n=0
x0=0.5
x1=1
dif=1
while dif>0.00000001:
    a=x1-f(x1)*(x1-x0)/(f(x1)-f(x0))
    n=n+1
    print(n,'    ',a)
    x0=x1
    x1=a
    dif=abs(x1-x0)
    
