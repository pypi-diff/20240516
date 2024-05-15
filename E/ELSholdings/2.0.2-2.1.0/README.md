# Comparing `tmp/elsholdings-2.0.2.tar.gz` & `tmp/elsholdings-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elsholdings-2.0.2.tar", last modified: Wed May 15 22:32:43 2024, max compression
+gzip compressed data, was "elsholdings-2.1.0.tar", last modified: Wed May 15 22:48:28 2024, max compression
```

## Comparing `elsholdings-2.0.2.tar` & `elsholdings-2.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 22:32:43.039997 elsholdings-2.0.2/
-drwxrwxrwx   0        0        0        0 2024-05-15 22:32:43.009420 elsholdings-2.0.2/ELSholdings/
-drwxrwxrwx   0        0        0        0 2024-05-15 22:32:43.034990 elsholdings-2.0.2/ELSholdings/kenwoo/
--rw-rw-rw-   0        0        0    45835 2024-05-15 22:32:07.000000 elsholdings-2.0.2/ELSholdings/kenwoo/xls2ppt.py
-drwxrwxrwx   0        0        0        0 2024-05-15 22:32:43.036996 elsholdings-2.0.2/ELSholdings.egg-info/
--rw-rw-rw-   0        0        0      425 2024-05-15 22:32:42.000000 elsholdings-2.0.2/ELSholdings.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2024-05-15 22:32:42.000000 elsholdings-2.0.2/ELSholdings.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 22:32:42.000000 elsholdings-2.0.2/ELSholdings.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-15 22:32:42.000000 elsholdings-2.0.2/ELSholdings.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      425 2024-05-15 22:32:43.038000 elsholdings-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       70 2024-05-13 23:52:45.000000 elsholdings-2.0.2/README.md
--rw-rw-rw-   0        0        0      366 2024-05-15 22:32:32.000000 elsholdings-2.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-15 22:32:43.039997 elsholdings-2.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-15 22:48:28.735103 elsholdings-2.1.0/
+drwxrwxrwx   0        0        0        0 2024-05-15 22:48:28.712938 elsholdings-2.1.0/ELSholdings/
+drwxrwxrwx   0        0        0        0 2024-05-15 22:48:28.730106 elsholdings-2.1.0/ELSholdings/kenwoo/
+-rw-rw-rw-   0        0        0    46067 2024-05-15 22:45:21.000000 elsholdings-2.1.0/ELSholdings/kenwoo/xls2ppt.py
+drwxrwxrwx   0        0        0        0 2024-05-15 22:48:28.732067 elsholdings-2.1.0/ELSholdings.egg-info/
+-rw-rw-rw-   0        0        0      425 2024-05-15 22:48:28.000000 elsholdings-2.1.0/ELSholdings.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2024-05-15 22:48:28.000000 elsholdings-2.1.0/ELSholdings.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 22:48:28.000000 elsholdings-2.1.0/ELSholdings.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-15 22:48:28.000000 elsholdings-2.1.0/ELSholdings.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      425 2024-05-15 22:48:28.734085 elsholdings-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       70 2024-05-13 23:52:45.000000 elsholdings-2.1.0/README.md
+-rw-rw-rw-   0        0        0      366 2024-05-15 22:47:29.000000 elsholdings-2.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-15 22:48:28.735103 elsholdings-2.1.0/setup.cfg
```

### Comparing `elsholdings-2.0.2/ELSholdings/kenwoo/xls2ppt.py` & `elsholdings-2.1.0/ELSholdings/kenwoo/xls2ppt.py`

 * *Files 2% similar despite different names*

```diff
@@ -548,22 +548,24 @@
     return None
 
 ############################################################################
 ############################################################################
 ############################################################################
 
 def remove_consecutive_zeros(df):
+    import pandas as pd
     # 첫 번째 행이 모두 0인 경우 삭제
     if (df.iloc[0] == 0).all():
         df.drop(df.index[0], inplace=True)
         # 재귀적으로 함수 호출하여 다음 첫 번째 행이 모두 0인 경우도 확인하고 삭제
         remove_consecutive_zeros(df)
 
 
 def stats_for_alives(df_Daily_NAV,date0):
+    import pandas as pd
     kr_cols= df_Daily_NAV.loc[date0].filter(regex=r'^KR')
     # 해당 칼럼에서 값이 0이 아닌 칼럼을 추출
     DD = kr_cols[kr_cols != 0] # 살아있는 넘들의 NAV
     if not DD.empty:
       Ret = (DD-10000)/100 # 리턴값(100% 환산값)
       Ret = Ret.astype('float64')
       # Ret_D 시리즈에서 최소값과 최대값에 해당하는 인덱스 찾기
@@ -572,32 +574,33 @@
       return Ret.describe(),min_Ret_index,max_Ret_index
 
     else:
       return None,None,None
 
 
 def pa_return_for_alives(df_Daily_NAV,final_date):
-  kr_cols= df_Daily_NAV.loc[final_date].filter(regex=r'^KR')
-  # 해당 칼럼에서 값이 0이 아닌 칼럼을 추출
-  DD = kr_cols[kr_cols != 0] # 살아있는 넘들의 NAV
-  df_alives=pd.DataFrame(DD)
-  df_alives.rename(columns={},inplace=True) # 칼럼이름 지우기
-  df_alives.columns=['조회된 날짜'] # 이름 새로 짓기
-
-  for code in df_alives.index:
-    first_date = df_Daily_NAV[code][df_Daily_NAV[code] != 0].first_valid_index()
-    duration = (pd.to_datetime(final_date) - first_date).days
-    df_alives.at[code,'발행일']=first_date
-    df_alives.at[code,'Duration']=duration
-    Ret= (df_alives.at[code,'조회된 날짜']-10000)/10000
-    Ret_pa=(1+Ret)**(365/duration)-1
-    df_alives.at[code,'절대수익율']=Ret
-    df_alives.at[code,'연환산수익율']=Ret_pa
+    import pandas as pd
+    kr_cols= df_Daily_NAV.loc[final_date].filter(regex=r'^KR')
+    # 해당 칼럼에서 값이 0이 아닌 칼럼을 추출
+    DD = kr_cols[kr_cols != 0] # 살아있는 넘들의 NAV
+    df_alives=pd.DataFrame(DD)
+    df_alives.rename(columns={},inplace=True) # 칼럼이름 지우기
+    df_alives.columns=['조회된 날짜'] # 이름 새로 짓기
+  
+    for code in df_alives.index:
+      first_date = df_Daily_NAV[code][df_Daily_NAV[code] != 0].first_valid_index()
+      duration = (pd.to_datetime(final_date) - first_date).days
+      df_alives.at[code,'발행일']=first_date
+      df_alives.at[code,'Duration']=duration
+      Ret= (df_alives.at[code,'조회된 날짜']-10000)/10000
+      Ret_pa=(1+Ret)**(365/duration)-1
+      df_alives.at[code,'절대수익율']=Ret
+      df_alives.at[code,'연환산수익율']=Ret_pa
 
-  return df_alives
+    return df_alives
 
 
 def stats_for_redeemed(df_Daily_NAV,input_date):
     import pandas as pd
     
     # date가 인덱스에 있는지 확인
     if input_date not in df_Daily_NAV.index: # 인덱스에 없는 날짜라면
@@ -667,14 +670,15 @@
             min_duration_index,
             max_duration_index,
             min_ret_pa_index,
             max_ret_pa_index)
 
 # 함수 작성
 def stats_for_redeemed_old(df_Daily_NAV,input_date):
+    import pandas as pd
     # date가 인덱스에 있는지 확인
     if input_date not in df_Daily_NAV.index: # 인덱스에 없는 날짜라면
         input_date=df_Daily_NAV.index[df_Daily_NAV.index < input_date].max() # 가장 가까운 앞 날짜 추출
     else: # 인덱스에 있다면 그냥 날짜객체로 반환
         input_date=pd.Timestamp(input_date)
 
     # 특정일을 나타내는 행에서 그 값이 0인 것들중 칼럼 이름이 KR로 시작하는 것들을 Series로 추출함
@@ -740,14 +744,15 @@
             max_duration_index,
             min_ret_abs_index,
             max_ret_abs_index)
 
 
 def hist_for_redeemded(df_Daily_NAV,input_date):
   import matplotlib.pyplot as plt
+  import pandas as pd
 
   # date가 인덱스에 있는지 확인
   if input_date not in df_Daily_NAV.index: # 인덱스에 없는 날짜라면
       input_date=df_Daily_NAV.index[df_Daily_NAV.index < input_date].max() # 가장 가까운 앞 날짜 추출
   else: # 인덱스에 있다면 그냥 날짜객체로 반환
       input_date=pd.Timestamp(input_date)
 
@@ -778,14 +783,15 @@
   ror_for_redeemed=df_redeemed.iloc[4,:]
   ror_for_redeemed.name='p.a.return'
 
   return ror_for_redeemed
 
 
 def get_issue_amount(df, date):
+    import pandas as pd
     # date가 문자열이라면 datetime 객체로 변환
     if isinstance(date, str):
         date = pd.to_datetime(date)
     # date가 datetime 객체가 아니라면 에러 메시지 출력
     elif not isinstance(date, pd.Timestamp):
         print("Error: 입력된 날짜가 올바르지 않습니다.")
         return None
@@ -800,14 +806,15 @@
     # 발행금액 합계와 계수 계산
     for i in idx:
         total_amount += df.at[i, '발행총액']
         total_sum += 1
     return total_sum,total_amount
 
 def info_for_redeemed(df,df_issued_summary,input_date):
+    import pandas as pd
     # date가 인덱스에 있는지 확인
     if input_date not in df.index: # 인덱스에 없는 날짜라면
         input_date=df.index[df.index < input_date].max() # 가장 가까운 앞 날짜 추출
     else: # 인덱스에 있다면 그냥 날짜객체로 반환
         input_date=pd.Timestamp(input_date)
     # 특정일을 나타내는 행에서 그 값이 0인 것들중 칼럼 이름이 KR로 시작하는 것들을 Series로 추출함
     zeros=df.loc[input_date][df.loc[input_date] == 0].filter(regex='^KR')
@@ -828,14 +835,15 @@
             continue # 다음 칼럼으로 이동
         redeemed_amount += df_issued_summary.at[col,'발행총액'] # 해당 종목의 발행총액을 더해줌
         redeemed_num += 1
 
     return redeemed_num,redeemed_amount/1e+9
 
 def sharpe_ratio_for_redeemed(df,rf, input_date):
+    import pandas as pd
     import numpy as np
     # date가 인덱스에 있는지 확인
     if input_date not in df.index: # 인덱스에 없는 날짜라면
         input_date=df.index[df.index < input_date].max() # 가장 가까운 앞 날짜 추출
     else: # 인덱스에 있다면 그냥 날짜객체로 반환
         input_date=pd.Timestamp(input_date)
```

