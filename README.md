# Monte-Carlo-Simulation

Stock prices follow a log-normal process:  dS=S(μdt+σdz) , where  μ  is a constant growth rate,  σ  is a constant volatility rate,  dt  is time interveral (1 month = 1/12), and  dz  is a normal distributed random variable with variance equal to  dt .

Start from a given  S0  (say, 100), we will have  St=St−1∗(1+μΔt+σΔt⎯⎯⎯⎯√Z)  for  t=1,2,...,N , where  Z  is a standard normal distributed variable.

The following code returns a numPy array with N+1 stock prices following the algorithm described above given input: N, μ, σ, Δt with default value 1 month (=1/12), and starting price S0 with default value 100.

And then generates a sequence of 60 monthly stock prices by calling function created above with  μ=6%,σ=10% ,  S0=100 . It will show 60 monthly returns based on this set of prices and compute the annualized return and annualized standard deviation.

Lastly, the code will simulate 1,000 and 10,000 times. And calculate the min, max, mean, and standard deviation at each month end (60 months).

You can always modify the inputs and number of simulations. 
