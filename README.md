- π Hi, Iβm @chu-saeyeon
- π Iβm interested in ...
- π± Iβm currently learning ...
- ποΈ Iβm looking to collaborate on ...
- π« How to reach me ...

<!---
chu-saeyeon/chu-saeyeon is a β¨ special β¨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
dist <- cars[,2]
hist(dist,
     main='Histogram for μ λκ±°λ¦¬',
     xlab='μ λκ±°λ¦¬',
     ylab='λΉλμ',
     border='blue',
     col='green',
     las=2,
     breaks=5)
boxplot(dist,main='μλμ°¨ μ λκ±°λ¦¬')
boxplot.stats(dist)
boxplot(Petal.Length~Species, data=iris, main='νμ’λ³ κ½μμ κΈΈμ΄')
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
     main='μ€λ-μ°λΉ κ·Έλν',
     xlab='μ€λ',
     ylab='μ°λΉ',
     col='red',
     pch=1)
vars <- c('mpg','disp','drat','wt')
target <- mtcars[,vars]
pairs(target,
      main='Multi Plots')
