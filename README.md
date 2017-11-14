# Understanding Uncertainty
Using interactive plots in Python to help readers make more sense of uncertainty in data samples.

This project follows from the points made in the paper [Sample-oriented task-driven visualizations: allowing users to make better, more confident decisions](https://drive.google.com/file/d/0B7Tj31nhk4BAeFJ1Y1lwQmpMQVk/view) by Ferreira, N., Fisher, D., & Konig, A. C. (2014, April). In Proceedings of the SIGCHI Conference on Human Factors in Computing Systems (pp. 571-580). ACM. [(video)](https://www.youtube.com/watch?v=BI7GAs-va-Q)

The uncertainty inherent in any estimate derived from a sample of a population is often overlooked when communicating findings in a report. Error bars factually communicate that uncertainty, but they do not help a reader intuitively understand the present uncertainty. Error bars are usually included as an after thought and the focus of the plot is still on the estimated values. The above cited paper explores the difficulties of conveying the level of uncertainty in estimates to readers and offers a few ways writers and researchers can improve their messaging.

This project builds two of the more involved methods the researchers suggest. The data for this project for each year is randomly genenerated from normal distributions with varying values of mean and standard deviation. Both plots show the data represented in a bar chart with error bars showing 95% confidence intervals for the mean of the data for each year.

The first plot focuses on the relationship between the population mean and a user-provided value. The coloring of each bar conveys the level of certainty a user should have regarding whether the population mean is above or below the given value based on the sample mean and sample variance. The more red the bar is, the more probable that the population mean is above the given y-value, while the more blue the bar, the more probable it is that the mean is below the given y-value. The user can click on the plot to change the y-value and the bars are automatically recolored.

![Image of first plot]
(https://github.com/henrywoody/Understanding-Uncertainty/blob/master/plot1.png)

The second plot examines the probability that the population mean falls within a range of y-values provided by the user. The user specifies the range and the more deeply red each bar is, the more probable it is that the population mean falls within the range given.

![Image of second plot]
(https://github.com/henrywoody/Understanding-Uncertainty/blob/master/plot2.png)
