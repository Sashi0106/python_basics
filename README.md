# python_basics
///
# Write a program to read a character untill * is entered.count the number of uppercase, lowercase, and numbers entered by the user..
ch=input("enter the character:")
n=u=l=0
if ch>='0' and ch<='9':
    n+=1
elif ch>='a' and ch<='z':
    l+=1
elif ch>'A' and ch<='z':
    u+=1
while ch!= '*':
    ch=input("enter any character!")
    if ch>='0' and ch<='9':
        n+=1
    elif ch>='a' and ch<='z':
        l+=1
    elif ch>'A' and ch<='z':
        u+=1
print("lower case characters:",l)
print("upper case characters:",u)
print("number characters:",n)
output:
enter the character: y
enter any character! A
enter any character! tag
enter any character! 6265
enter any character! *
lower case characters: 2
upper case characters: 0
number characters: 1
///
# simple for loop (string)
str= 'cheetah'
for i in str:
    print(i,end=' ')
output:
    c h e e t a h 
///
#list of strings
s=['cat','dog','fish']
for pet in s:
    print(pet)
output:
cat
dog
fish
///
#for with in range
n= int(input("enter the value of n"))
for i in range(21,n+1,-1):
    print(i,end=' ')
for i in range(n,0,-2):
    print(i,end=' ')
output:
enter the value of n 10
21 20 19 18 17 16 15 14 13 12 10 8 6 4 2 
///
# code for printing multiplication table of n, where n is entered by the user
n=int(input())
for i in range(1,11):
    print(n,'x',i,'=',n*i)
  OUTPUT:
   2
2 x 1 = 2
2 x 2 = 4
2 x 3 = 6
2 x 4 = 8
2 x 5 = 10
2 x 6 = 12
2 x 7 = 14
2 x 8 = 16
2 x 9 = 18
2 x 10 = 20
///
#program to display all the leasp years from 1900 to 2101
st=int(input("enter the starting year:"))
ed=int(input("enter the ending year:"))
for i in range(st,ed+1):
    if i%4==0:
        print(i,end=' ')
output:
enter the starting year: 1900
enter the ending year: 2101
1900 1904 1908 1912 1916 1920 1924 1928 1932 1936 1940 1944 1948 1952 1956 1960 1964 1968 1972 1976 1980 1984 1988 1992 1996 2000 2004 2008 2012 2016 2020 2024 2028 2032 2036 2040 2044 2048 2052 2056 2060 2064 2068 2072 2076 2080 2084 2088 2092 2096 2100 
///
# Numbers in series
n=int(input("enter the value of n:"))
s=0.0
for i in range(1,n+1):
    a=1.0/(i**2)
    s+=a
print(s)
output:
enter the value of n: 5
1.4636111111111112
///
n=int(input("enter the value of n:"))
s=0.0
for i in range(1,n+1):
    a=i**i/(i)
    s+=a
print(s)
output:
enter the value of n: 5
701.0
///
#generating a calender manually
sday=int(input("enter the start day of the moneth(1-7)L"))
numdays=int(input("enter the number of days"))
print("Sun  Mon  Tue  Wed  Thu  Fri  Sat")
print("-----------------------------")
for i in range(sday+1):
    print(end="    ")
i=sday-1
for j in range (1,numdays+1):
    if i>6:
        print()
        i=1
    else:
        i+=1
    print(str(j)+"  ", end=' ')
output:
enter the start day of the moneth(1-7)L 5
enter the number of days 31
Sun  Mon  Tue  Wed  Thu  Fri  Sat
-----------------------------
                        1   2   3   
4   5   6   7   8   9   10   
11   12   13   14   15   16   17   
18   19   20   21   22   23   24   
25   26   27   28   29   30   31   
///
