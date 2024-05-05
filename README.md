# R-Performance-At-Work
In this project, we use RStudio to make inferences about “performance at work” data. First, we import the data set from Excel with the name PW and calculate a column with the average time to make each note by day.
![r1](https://github.com/migutierrez940605/R-Performance-At-Work/assets/143429236/5d581da3-e328-405e-b7f7-7b8382cb0b9f)

Second, we can visualize the data with a boxplot graphic to detect outliers’ data and variability.
![r2](https://github.com/migutierrez940605/R-Performance-At-Work/assets/143429236/add5c10c-d3d1-4691-a74a-d60ed36a2d6b)

Return
![r3](https://github.com/migutierrez940605/R-Performance-At-Work/assets/143429236/4621fb8e-c4f1-492a-8c16-634caee99256)

The graphic shows the outliers’ data, but we must select these numbers to identify them.  
![r4](https://github.com/migutierrez940605/R-Performance-At-Work/assets/143429236/bfc0a9fa-77c3-48af-b478-4449eef345c1)

Then, by an expert's decision, we remove the first data from the vector "o" in which the outlier data are.
![r5](https://github.com/migutierrez940605/R-Performance-At-Work/assets/143429236/deaed7bc-ac32-4c32-8fb0-0672cacd1047)

Next, we use the Shapiro Test to prove if the “or” vector is normally distributed.
![r6](https://github.com/migutierrez940605/R-Performance-At-Work/assets/143429236/1ade6549-7791-466f-8a06-4f5d06a4fa61)

The p-value of the test turns out to be 0.8899. Since this value is not less than 0.05, we can assume the “or” vector comes from a population that is normally distributed. Therefore, we can use the parametric t-hypothesis test for small samples. We select as Null Hypothesis µ=4, the Alternative Hypothesis as µ≠4, and α=0.05.
![r7](https://github.com/migutierrez940605/R-Performance-At-Work/assets/143429236/1d3e672b-b015-4459-a0cb-82f389055619)

The p-value of the test turns out to be 0.2479. Since this value is not less than 0.025, there is not enough evidence to reject the Null Hypothesis (µ=4). Also, we can see that the populate parameter is between 3.761742 and 4.064084 with a confidence of 95%.
