# Bayesian
To import the data, you need to change the file address that suits your computer 
This import data is based on the data file Kasha sent me with 288 text files. With more data need to have improvement with the import data function.  
but the key idea is to create a long-format data file with all participants in one condition. 

the normal distribution may not be the best distribution to set the prior. the prior set with normal diribution is too narrow compared to the posterior. 

When you run the loop it will appear error like this: Semantic error in 'string', line 27, column 28 to column 30: Identifier 'p3' not in scope.

the loop itself has no problem. however, the stan function since unable to call the posterior from the previous fit model by index (e.g. as.numeric(posterior1[1,1])) (can only do by inputting the posterior number manually although they were the same thing).
I tried to fix the error these two days but I failed to do so (some people say can be fixed by restarting the R session but i tried it doesn't work). 