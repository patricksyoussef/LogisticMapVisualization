# Logistic Map Visualization

## Usage

Usage is quite simple, you just need to modify the parameters in the code shown below:

```python
num_base_iters = 1000   # Base iterations to reach steady-state, 1000 is plenty
num_final_iters = 500   # How many iterations to save for plotting
r_start = 2.9           # The lower bound of R values to plot for
r_stop = 3.99           # The upper bound of R values to plot for
n = 1000                # Number of equally space r values
```

If you want to read more about the path to the final code and more information on the equation itself, read ahead.

## What Is The Logistic Map?

The [logistic map](https://en.wikipedia.org/wiki/Logistic_map) is a math equation that was often used to describe population growth in natural systems, but more commonly is cited as an interesting case of chaotic nature arising out of simple mathematics.

The equation is a recursive relation wherein the updated value on the left hand side is the new population some time-step. For a typical system we would expect this to steady state to some value over many iterations. For values of the growth constant R that are just greater than ~3 the stead-state population oscillates between two values and as R progresses becomes more and more chaotic.

## Visualization

Knowing the information of the prior section I decided to plot the equation for a `linspace` of R values and save N samples after an initial necessarily large set of iterations to get past the initial growth. These samples were plotted against each R value, so for a single steady-state value we'd expect a point and for chaotic populations we'd begin to build a field of densities depending on the occurrence of points. This yield the below:

<img src="imgs/plotsimple.png" width="60%">

Which I find to be quite beautiful, and now I wanted it as a desktop background.

## Improving The Visualization

I improved the artistic nature of the plot by increasing the number of samples and doing a black and white variant with not plot axes or grids. This is the current code in this repo. Below is the result of the visualization zoomed in on a particular region:

![Refined Image Whole](imgs/map_full.png)
![Refined Image Close](imgs/crossings.jpg)

## Questions

Please let me know if you have any questions and I hope you like it!