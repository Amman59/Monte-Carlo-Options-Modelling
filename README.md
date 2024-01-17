# 2nd-Project
Random coding problems, which I hopefully solve. 


I found an interesting peice of code online which looks at using the Black-Scholes-Merton Option Pricing model and using a normally distributed set of random numbers to test what the value of a European Style call option is worth. The second block of code is a combination of the plotting code from my previous project and the pricing model, just to let me observe how the distribution would look.Plotting this was an odd task, given that the value of C0 in this model is the mean value and this would only provide a single point. Thus I decided to use the hT values and then adjust them by appying the function to generate ST, without finding the mean value. 

The graph now shows the value of the option relative to the index i.e if the value of hT is 8 then the diagram will show a value of 108 for ST. I have added some of own variables, as I had difficulties plotting and wanted to find out at which point the plot would have these difficulties. These values that I have used are exact values rather than variables so as to make finding the problem easier, so if the condition of the model were to be changed I would have to manually find all the values in the code and change them. It may not be pretty, but at least I can plot the set of data points and come to valid conclusions as a result. Because my variables come from a different seed, when I plot both against each other I can see the distribution is different - however as this is a Monte-Carlo model, the law of large numbers has meant that the mean value, in this case the price of the option, is the same in both seeds. 

My knowledge of the Black-Scholes-Merton model is severly limited and I am trusting the 'Open source' formula to be correct. I am aware that this model can only be used on European stlye options due to the nature of being able to exercise the options only at expiration, and also relies on long term 'Ceteris paribus'. The assumptions do limit this model, and this reminds me of a joke that my physical dynamics professor used to say - 'assume a spherical cow'. I first heard of the model when interviewing at UBS and one of the job description notes said 'Have you done you reading on the Black-Scholes?' so I decided I had better do my reading!
