## Secant Lines and Average Rates of Change

Linear functions are some of the most fundamental functions in mathematics. They are used often to describe the behavior of other (more complex) functions. Fairly often we want to estimate how fast the state of a system has changed from some point in time to some other time in the future. This provides a sense of the system's _tendency_ (its _trend_) --- how the system is behaving during a certain period of time. The system may be increasing its state very rapidly, or more moderately, of perhaps barely. The system might not be changing at all. Or perhaps the system's state could be decreasing very rapidly, moderately, or very slightly. The system could also keep its current state into another (adjacent) point in time.

**Example: Estimating prevalence of a virus in a population**

Many state agencies use the _positivity rate_ (number of positive tests per total number of tests) to assess how widespread a virus is in some demarcation. The state of Rhode Island Department of Health reports weekly COVID-19 positivity rates (see [https://ri-department-of-health-covid-19-data-rihealth.hub.arcgis.com/](https://ri-department-of-health-covid-19-data-rihealth.hub.arcgis.com/)). The table below shows weekly positivity rates for COVID-19 in RI from the week of Nov 27, 2021 to the week of Jan 15, 2022.

<table width="640"><tbody><tr><td width="110">t</td><td width="70">1</td><td width="64">2</td><td width="68">3</td><td width="68">4</td><td width="68">5</td><td width="64">6</td><td width="64">7</td><td width="64">8</td></tr><tr><td>Week of</td><td>27-Nov</td><td>4-Dec</td><td>11-Dec</td><td>18-Dec</td><td>25-Dec</td><td>1-Jan</td><td>8-Jan</td><td>15-Jan</td></tr><tr><td>Positivity rate (%)</td><td>4.1</td><td>5.3</td><td>5.7</td><td>6.2</td><td>7.1</td><td>16.4</td><td>21.2</td><td>18.7</td></tr></tbody></table>
<p></p>
To assess the tendency of COVID-19 from a given week $$A$$ to a later week $$B,$$ we compare how much the positivity rate ($$PR$$ for short) changed from week $$A$$ to week $$B$$ by taking the difference $$PR(B) - PR(A)$$ (later value minus earlier value).<p></p>

Questions for you:

1.  Did the $$PR$$ change from the week of Thanksgiving (Nov 27) to the week of Christmas (Dec 25)? If so, by how much? How many weeks separate these two estimates?
2.  What about from the week of Christmas to the week of New Year's day? The last week of available data?
3.  Use Desmos or Geogebra (or some other graphing tool you like) to visualize these data. What can you say about the $$PR$$ in RI in the last several weeks? Are there any intervals of special interest? See https://publichealth.jhu.edu/2020/covid-19-testing-understanding-the-percent-positive.

As you can see, a different number of weeks separate the two pairs of estimates in questions $$1$$ and $$2$$ above. To account for those differences, we often $$normalize$$ the estimates by dividing the change in state by the number of units of time elapsed. This is called an _average rate of change_ of the system's state from time $$A$$ to time $$B.$$ Some times we write $$AV_{[A,B]}$$ for short.

More questions for you:

4.  Compute the average rate of change for the time periods in questions $$1$$ and $$2$$ above.
5.  For the points in questions $$1$$ and $$2$$ above compute the slope of the straight line that passes through those points. These lines are called _secant lines._ Did you get any familiar results?
6.  Use a spreadsheet like Excel to compute the weekly average rate of change for each consecutive pair of weeks. Paste your data from the spreadsheet into Desmos and visualize it. How could you interpret this graph in terms of the state of this system?
