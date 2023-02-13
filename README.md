# QUIZ-PROGRAM
quiz program in python
#QUIZ PROGRAM
def q_1():
  print("1,Who developed Python Programming Language?")
  print("a) Wick van Rossum")
  print("b)Guido van Rossum")
  Answer="Guido van Rossum"
  choose =str(input("choose the correct answer:"))
  score=0
  if(choose==Answer):
   score=2
  else:
   score=-1
  return(score)
def q_2():
  print("2)Is Python case sensitive when dealing with identifiers?")
  print("a) No")
  print("b)machine dependent")
  Answer="No"
  choose =str(input("choose the correct answer:"))
  score=0
  if(choose==Answer):
    score=2
  else:
    score=-1
  return(score)
def q_3():
  print("3) Which of the following is used to define a block of code in Python language?")
  print("a)Indentation")
  print("b)Brackets")
  Answer="Indentation"
  choose =str(input("choose the correct answer:"))
  score=0
  if(choose==Answer):
   score=2
  else:
   score=-1
  return(score)
def q_4():
  print("4)Which of the following functions is a built-in function in python?")
  print("a)sqrt()")
  print("b)print()")
  Answer="print()"
  choose =str(input("choose the correct answer:"))
  score=0
  if(choose==Answer):
    score=2
  else:
    score=-1
  return(score)
def q_5():
  print("5) Which of the following is not a core data type in Python programming?")
  print("a)Lists")
  print("b)Class")
  Answer="Class"
  choose = str(input("choose the correct answer:"))
  score=0
  if(choose==Answer):
    score=2
  else:
    score=-1
  return(score)
A1=q_1()
A2=q_2()
A3=q_3()
A4=q_4()
A5=q_5()
ANS=A1+A2+A3+A4+A5
print("The total mark is:",ANS)

import pandas as pd
song_details =pd.DataFrame({
'Index':[1,2,3,4,5,6,7,8,9,10],
'Id': ['s1','s2','s3','s4','s5','s6','s7','s8','s9','s10'],
'Year':[2010,2012,2003,2000,2001,2016,2015,2021,2022,2001],
'Rank':[1,2,4,5,6,7,9,3,8,10],
'Album_name':['pookal pookum tharunam','Kaal Mulaitha Poovae','Nenjodu','thozha thoza',
              'enna solla pogirai','jithu jiladi','alagu','karunan','kadal','nila'],
'Music_dir':['Gv',' Harris Jayaraj','Yuvan Shankar Raja','Arr','Yugendran','Balachandran',
             'ajith','dhanush','ilaiyaraja','gv prakash'],
'Singer':[' Andrea Jeremiah','unnikrishnan','Shankar Mahadevan','Yugendran',
          'Gv','malar','kaviya','ram','mani','krishnan'],
'Type':['melody','jazz','meloady','melody','melody','melody','jazz','hiphop','melody','hiphop'],
})
song_details

print('Top 10 songs in 2022')
display(song_details.loc[song_details['Year']==2022])

print('classify melody and jazz')
display(song_details.loc[song_details['Type'].str.contains('melody|jazz')])

print('Sort based on year rank')
display(song_details.sort_values(['Rank']))
