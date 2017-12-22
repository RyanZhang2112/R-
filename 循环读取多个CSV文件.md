```{r}
> setwd("D:/工作/实车数据/观致数据/sourceData_16/LLNC1AAB4FA000781")  
> getwd  
> a = list.files()  
> n = length(a)  
> merge.data <- read.csv(file = a[1], header = T）  
> for(i in 2:n){  
>   new.data <- read.csv(file = a[2], header = F)  
>   merge.data = rbind(merge.data, new.data)  
>   }  
> write.csv(merge.data, file = "merge_data.csv", row.names = F) #生成CSV文件  
```
