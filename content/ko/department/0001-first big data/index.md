---
title: 빅데이터이해및활용 과제 1
date: 2023-09-02
---

전라북도 시민들의 건강상태 데이터를 분석하는 활동

<!--more-->
```
## 빅데이터이해및활용_컴퓨터공학부_20201680_안현_과제_1

data <- read.csv("국민건강보험공단_건강검진정보_20211231.csv")
data

# 전라북도의 시도코드 = 45
JB <- subset(data, SIDO == 45)
JB
# 40대의 연령대코드 = 9,10
JB_40 <- subset(JB, AGE_GROUP == 9 | AGE_GROUP == 10)
JB_40

# 남성은 파란색, 여성은 빨간색
color <- c("blue", "red")
col.idx <- c(JB_40$SEX)
color[col.idx]

# 남성은 세모, 여성은 네모
pchar <- c(17, 15)
pch.idx <- c(JB_40$SEX)
pchar[pch.idx]

# 범례를 위한 문자 설정
legeno <- c("남성", "여성")
lgd.idx <- c(JB_40$SEX)
legeno[lgd.idx]

plot(JB_40$BP_HIGH, JB_40$BP_LWST, col = color[col.idx], pch = pchar[pch.idx])
legend("topleft", legend = legeno, col = color, pch = pchar)

cor(JB_40$BP_HIGH, JB_40$BP_LWST)
# 수축기 혈압과 이완기 혈압의 상관관계는 0.8007881입니다.
# 양의 상관관계이며, 상관성이 꽤 높다고 볼 수 있습니다.
# 수축기 혈압이 증가하면 이완기 혈압도 증가하는 추세이며, 그 역도 성립합니다.
# 수축기 혈압이 감소하면 이완기 혈압도 감소하는 추세이며, 그 역도 성립합니다.
```