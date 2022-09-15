# TIL

# 보건의료데이터마이닝 파이썬

> Jupyter Notebook, Anaconda3 : 주석은 # 문자를 이용하여 달 수 있음.   
> 주석은 not effect to Run  

#  Data Type, Basic Standard Function, Numpy / Pandas  

  정수형 = int, 실수형 = float, 복소수형 = complex  
  
  INDEXING, SLICING - String_test
  
  if 조건문 : 조건에 맞으면 수행, 조건에 맞지 않으면 건너뜀  
  
  ```
  score = 88
  if score >= 90:
      print("A")
  elif score < 90 and score >=80 :
      print("B")
  else:
      print("C")
  ```
     
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
            
#05_26 보건의료데이터마이닝 Class : Numpy
  NUMPY : 행렬이나 대규모 다차원 배열을 쉽게 처리할 수 있게 해주는 파이썬의 라이브러리, Pandas와 Matplotlib 기반
  
    import numpy as np
    data1 = [1,2,3,4,5]
    arr1 = np.array(data1)
    arr1
    
  array([1,2,3,4,5)]
  
  np.exp(array) : 지수함수, np.log(array) : 자연로그, np,sign(array) : 부호계산
  np.round(arr1) : 반올림 계산, np,cos(arr1) : 삼각함수 cosine 계산, np.isnan(arr1) : boolean 테스트
 
 
>PANDAS : 데이터 조작 및 분석을 하기 위한 파이썬 패키지(라이브러리)
  pandas를 이용해 파일 불러오기
    데이터 파일 저장 위치 : C드라이브 - 사용자 - ms400
    titanic_df = pd.read_csv("titanic.csv:)
    titanic_df
 
Matplotlib : 데이터 시각화를 위한 파이썬 library,  논문 발행 수준의 높은 품질의 그림을 그릴 수 있다.
  import matplotlib.pyplot as plt

    cross_tab_prop.plot(
    kind='bar',
    color=["b","r"],
    stacked=True,
    figsize=(15,6))
    plt.legend(loc="upper right", ncol=1)
    plt.ylabel("Probablility of 'survived' at given status")



    for n, x in enumerate([*cross_tab.index.values]):
    for (proportion, count, y_loc) in zip(cross_tab_prop.loc[x],
                                          cross_tab.loc[x],
                                          cross_tab_prop.loc[x].cumsum()):
        plt.text(x=n-0.1,
                y=(y_loc-proportion)+(proportion/2),
                 s=f'{count}\n({np.round(proportion*100, 1)}%)',
                 color="black",
                 fontsize=12,
                 fontweight="bold")
    plt.show()



# 의사결정나무 Classification, Machine learning
  
     import pandas as pd #PANDAS library
     import numpy as np #NUMPY library
     import matplotlib.pyplot as plt #matploylib library
  
      titanic_df = pd.read_csv("titanic.csv")
      titanic_df
  
  



    



