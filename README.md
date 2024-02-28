# Rprogramming
#Posting Rprogramming Code
datasets::airquality
df=datasets::airquality
head(airquality,10)
view(airquality)
airquality[,c(1,2)]
airquality[,1:2]
df<-airquality[,-6]
##Plot##
plot(airquality$Wind)
plot(airquality$Temp)
plot(airquality$Temp,airquality$Wind, type="o")
plot(airquality$Wind, xlab="Ozone Conc", ylab="Instances", main="Ozone levels in NY City", col="orange")
#Histogram#
hist(airquality$Temp, col="green")
df=datasets::quakes
quakes[, 1:2]
skewness(airquality$Ozone,na.rm=T)
hist(airquality$Ozone)
kurtosis(airquality$Ozone, na.rm=T)
plot.new()
plot(density(airquality$Ozone, na.rm=T), col='purple')
