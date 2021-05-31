- 👋 Hi, I’m @chu-saeyeon
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
chu-saeyeon/chu-saeyeon is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
dist <- cars[,2]
hist(dist,
     main='Histogram for 제동거리',
     xlab='제동거리',
     ylab='빈도수',
     border='blue',
     col='green',
     las=2,
     breaks=5)
boxplot(dist,main='자동차 제동거리')
boxplot.stats(dist)
boxplot(Petal.Length~Species, data=iris, main='품종별 꽃잎의 길이')
par(mfrow=c(1,3))
boxplot(table(mtcars$carb),
        main='Barplot of Carburetors',
        xlab='#of carburetors',
        ylab='frequency',
        col='blue')
boxplot(table(mtcars$cyl),
        main='Barplot of Cylender',
        xlab='#of cylender',
        ylab='frequency',
        col = 'red')
boxplot(table(mtcars$gear),
        main='Barplot of Grar',
        xlab='#of gears',
        ylab='frequency',
        col='green')
par(mfrow=c(1,1))
wt <- mtcars$wt
mpg <- mtcars$mpg
plot(wt,mpg,
     main='중량-연비 그래프',
     xlab='중량',
     ylab='연비',
     col='red',
     pch=1)
vars <- c('mpg','disp','drat','wt')
target <- mtcars[,vars]
pairs(target,
      main='Multi Plots')
