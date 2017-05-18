# TEBASIIMA JOHN 16/U/1184
def dob(x,y,z):
     a=26
     b=6
     c=2016
     n=(b-y)
     if x>31:
             print("invalid")
             return
     if y>12:
            print("invalid")
            return
     if n==1:
         r=(a-x)+31*(b-y)+365*(c-z)
     elif n==2 or n==-2:
         r=(a-x)+61/2*(b-y)+365*(c-z)
     elif n==-3 or n==3:
         r=(a-x)+92/3*(b-y)+365*(c-z)
     elif n==-4:
         r=(a-x)+122/4*(b-y)+365*(c-z)
     elif n==-5:
         r=(a-x)+153/5*(b-y)+365*(c-z)
     elif n==-6:
         r=(a-x)+183/6*(b-y)+365*(c-z)
     elif n==-1:
         r=(a-x)+30*(b-y)+365*(c-z)
     elif n==5:
         r=(a-x)+152/5*(b-y)+365*(c-z)
     elif n==0:
         r=(a-x)+365*(c-z)
     elif n==4:
         r=(a-x)+121/4*(b-y)+365*(c-z)
     m=(c-z)//4
     g=r%7
     f=(g+m)%7
     l=f//1
     q=(c-z)/4
     if q!=m:
          l=l+1
     if l==0 or l==7:
            print("You are born on Sunday")
     if l==1:
            print("You are born on Saturday")
     if l==2:
            print("You are born on Friday")
     if l==3:
            print("You are born on Thursday")
     if l==4:
            print("You are born on Wednesday")
     if l==5:
            print("You are born on Teusday")
     if l==6:
            print("You are born on Monday")

dob(18,5,2017)
