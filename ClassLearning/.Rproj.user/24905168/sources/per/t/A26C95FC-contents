#Data Preprocessing in R
data <- read.csv("USA_cars_datasets.csv")
head(data)
summary(data)
tail(data)
dim(data)

#Check if ther's null values
colSums(is.na(data))

#Descriptive stats
mean(data$price)
median(data$price)
max(data$price)
quantile(data$price)
var(data$price)
sd(data$price)

print(data$price[166])


#Most expensive car with lowest mileage



  

print(data$price)

for (i in data$price){
  if (i > 10000){
    data$expensive <- 'yes'
  } else{
    data$expensive <- 'no'
  }
}

head(data)

#Car model in the year 2020 with the highest price
maxTwenty <- max(data$price[data$year == '2020'])
data$model[data$price == maxTwenty]


carprice <- max(data$price)
lowestmileage <- min(data$mileage)
answer <- ''
for (i in 1:2499){
  if ((data$mileage[i] == lowestmileage) || (data$price == carprice)){
    answer <- paste(answer,data$brand[i])
  }
}

answer


#In what year did we have the oldest car

oldestcar <- min(data$year)

oldestcar

#Most frequent car

max(table(data$brand))

max(table(data$color))


