---
title: 빅데이터이해및활용 과제 2
date: 2023-09-03
---

시, 도 별 인구밀도를 트리맵으로 그려보는 활동

<!--more-->
```
## 빅데이터이해및활용용_컴퓨터공학부_20201680_안현_과제_2

#사전 준비를 해줍니다.
setwd("C:/Users/USER/OneDrive/바탕 화면/안현/2-2/과제/빅데이터")
install.packages("treemap")

# 데이터를 다운로드 받습니다.
# 시도의 이름이 너무 길어서 임의로 수정했습니다.
data1 <- read.csv("성_및_연령별_인구와_인구밀도_20231128223048.csv")
data2 <- read.csv("인구_천명당_의료기관병상수_시도_시_군_구__20231128222621.csv")

data1
data2

# 21년도의 인구 수 / 20년도의 면적 = 인구 밀도로 만들어서 데이터 프레임에 더해줍니다.
data3 <- merge(data1, data2)
data3

data3$DENS <- data3$POPUL / data3$AREA
data3


# 트리맵을 이용하여 표현해줍니다.
# plots 창의 크기에 따라 트리맵의 모양이 달라집니다.
library(treemap)
treemap(data3,
        index = "SIDO",
        vSize = "DENS",
        vColor = "BED",
        type = "value",
        title = "Medical infrastructure",
        palette = "RdBu")
```