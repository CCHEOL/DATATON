# 구글어스 경로 데이터 전처리
###### 현장조사를 통해 얻은 캠퍼스 경로 중 사용할 수 없는 *빨간색 레벨* 의 경로를 제거
---

### 실행 코드

```Python
import pandas as pd

df=pd.read_excel(r'C:\Users\rlacj\OneDrive\바탕 화면\구글어스 통합본.xlsx')

df = df[df['레벨 분류'].isin(['노', '초'])]

df.to_excel('구글어스 전처리.xlsx')
```
