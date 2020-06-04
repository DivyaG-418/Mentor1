# Q1

import pandas as pd

df = pd.read_csv("C:/Users/satya/Desktop/Python/Daily Assig/Automobile_data.csv")

strt = df.head(5)

end = df.tail(5)

print(strt)

print(end)


# Q2

print(df.isnull())


# Q3

print(df[["company","price"]][df["price"]==df["price"].max()])


# Q4

print(df[df["company"] == "toyota"])


# Q5

print(df["company"].value_counts())


# Q6

print(df.groupby("company")["price"].max())


# Q7

print(df.groupby("company")["average-mileage"].mean())


# Q8

print(df.sort_values("price"))


# Q9

f1 = GermanCars = {'Company': ['Ford', 'Mercedes', 'BMV', 'Audi'], 'Price': [23845, 171995, 135925 , 71400]}

f2 = japaneseCars = {'Company': ['Toyota', 'Honda', 'Nissan', 'Mitsubishi '], 'Price': [29995, 23600, 61500 , 58900]}


df1 = pd.DataFrame(f1)

df2 = pd.DataFrame(f2)

df1

df2

print(pd.concat([df1,df2],axis=0,keys=["GermanCars","JapaneseCars"]))



# Q10

d1 = Car_Price = {'Company': ['Toyota', 'Honda', 'BMV', 'Audi'], 'Price': [23845, 17995, 135925 , 71400]}

d2 = car_Horsepower = {'Company': ['Toyota', 'Honda', 'BMV', 'Audi'], 'horsepower': [141, 80, 182 , 160]}

df1 = pd.DataFrame(d1)

df2 = pd.DataFrame(d2)

df1

df2

print(pd.merge(df1,df2))

