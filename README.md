# TIL
# 인프런 파이썬 강의

# 보건의료데이터마이닝 파이썬
#05_05 보건의료데이터마이닝 Class
Jupyter Notebook, Anaconda3 : 주석은 # 문자를 이용하여 달 수 있음. 주석은 not effect to Run

#05_19 보건의료데이터마이닝 Class : Data Type, Basic Standard Function, Numpy / Pandas
  정수형 = int, 실수형 = float, 복소수형 = complex
  INDEXING, SLICING - String_test
  
  if 조건문 : 조건에 맞으면 수행, 조건에 맞지 않으면 건너뜀
  score = 88
  if score >= 90:
      print("A")
  elif score < 90 and score >=80 :
      print("B")
  else:
      print("C")
     
FOR 구문 : 가장 기본적인 반복문으로, 리스트나 튜플 같은 시퀀스형을 이용하여 반복
list_example = ["ABCDE", "Phython", "for loop"]
for s in list _example :
  print(s, len(s))
  
  LIST, TUPLE 자료형
   List - 순서를 가지는 객체들의 집합
          Sequence 자료형이며 변경 가능(mutable)형임
          []로 표현함
   Tuple - 순서를 가지는 객체들의 집합
            Sequence 자료형이며 변경 불가능(immutable)형임
            ()로 표현

