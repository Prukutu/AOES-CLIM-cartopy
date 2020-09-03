---
title: Visualizing Tabular Data
teaching: 0
exercises: 0
questions:
- "How can I visualize tabular data in Python?"
- "How can I group several plots together?"
objectives:
- "Plot simple graphs from data."
- "Group several graphs in a single figure."
keypoints:
- "Use the `pyplot` module from the `matplotlib` library for creating simple visualizations."
---

## Visualizing data
The mathematician Richard Hamming once said, "The purpose of computing is insight, not numbers," and
the best way to develop insight is often to visualize data.  Visualization deserves an entire
lecture of its own, but we can explore a few features of Python's `matplotlib` library here.  While
there is no official plotting library, `matplotlib` is the _de facto_ standard.  First, we will
import the `pyplot` module from `matplotlib` and use two of its functions to create and display a
heat map of our data:

~~~
import matplotlib.pyplot
image = matplotlib.pyplot.imshow(data)
matplotlib.pyplot.show()
~~~
{: .language-python}

![Heatmap of the Data](../fig/inflammation-01-imshow.svg)

Blue pixels in this heat map represent low values, while yellow pixels represent high values.  As we
can see, inflammation rises and falls over a 40-day period.  Let's take a look at the average inflammation over time:

~~~
ave_inflammation = numpy.mean(data, axis=0)
ave_plot = matplotlib.pyplot.plot(ave_inflammation)
matplotlib.pyplot.show()
~~~
{: .language-python}

![Average Inflammation Over Time](../fig/inflammation-01-average.svg)

Here, we have put the average inflammation per day across all patients in the variable `ave_inflammation`, then
asked `matplotlib.pyplot` to create and display a line graph of those values.  The result is a
roughly linear rise and fall, which is suspicious: we might instead expect a sharper rise and slower
fall.  Let's have a look at two other statistics:

~~~
max_plot = matplotlib.pyplot.plot(numpy.max(data, axis=0))
matplotlib.pyplot.show()
~~~
{: .language-python}

{% include links.md %}
