Download Link: https://assignmentchef.com/product/solved-ml-homework3-random-data-generator
<br>
<strong>                                                                                  </strong>

<ol>

 <li><strong> Random Data Generator </strong> a. Univariate gaussian data generator</li>

</ol>

Expectation value or mean:

Variance:

Output: A data point from

<a href="https://en.wikipedia.org/wiki/Normal_distribution#Generating_values_from_normal_distribution"><strong>Generatin</strong></a><a href="https://en.wikipedia.org/wiki/Normal_distribution#Generating_values_from_normal_distribution"><strong>g</strong></a><a href="https://en.wikipedia.org/wiki/Normal_distribution#Generating_values_from_normal_distribution"><strong> values from normal distribution</strong></a>

You have to handcraft your geneartor based on one of the approaches given in the hyperlink.

You can use uniform distribution function (Numpy)

<h1>2.    Sequential Estimator</h1>

Sequential estimate the mean and variance

Data is given from the univariate gaussian data generator (1.a). Input:        as in (1.a) Function:

Call (1.a) to get a new data point from

Use sequential estimation to find the current estimates to               and

Repeat steps above until the estimates converge.

Output: Print the new data point and the current estimiates of                  and  in each iteration.

Notes

You should derive the recursive function of mean and variance based on the sequential esitmation.

Hint: <a href="https://en.wikipedia.org/wiki/Algorithms_for_calculating_variance#Online_algorithm"><strong>Online al</strong></a><a href="https://en.wikipedia.org/wiki/Algorithms_for_calculating_variance#Online_algorithm"><strong>g</strong></a><a href="https://en.wikipedia.org/wiki/Algorithms_for_calculating_variance#Online_algorithm"><strong>orithm</strong></a>

Sample input &amp; output (           <strong><em>for reference only</em></strong>         )

1 Data point source function: N(3.0, 5.0)

2

<ul>

 <li>Add data point: 234685454257290</li>

 <li>Mean = 408993960833291 Variance = 0.030383455464755956</li>

 <li>Add data point: 519242879651157</li>

 <li>Mean = 445743600439247 Variance = 1.875958150575018</li>

 <li>Add data point: 347113997201991</li>

 <li>Mean = 171086199629932 Variance = 1.633278676389248</li>

 <li>Add data point: 979491998496083</li>

 <li>Mean = 532767359403163 Variance = 8.723325264636875</li>

 <li>Add data point: 603448448693051</li>

 <li>Mean = 544547540951477 Variance = 7.270131583917285</li>

 <li>Add data point: 127197937610908</li>

 <li>Mean = 627783311902824 Variance = 6.273110519038578</li>

 <li>Add data point: 992735798186870</li>

 <li>Mean = 798402372688330 Variance = 5.692747751482052</li>

</ul>

17

18 …

19

<ul>

 <li>Add data point: 233592159021013</li>

 <li>Mean = 961576104513964 Variance = 5.045715437349161</li>

 <li>Add data point: 529990930040463</li>

 <li>Mean = 961883688294010 Variance = 5.043159812425648</li>

 <li>Add data point: 125210345431449</li>

 <li>Mean = 960890354955524 Variance = 5.042255747918937</li>

</ul>

<h1>3.    Baysian Linear regression</h1>

Input

The precision (i.e., b) for initial prior

All other required inputs for the polynomial basis linear model geneartor (1.b)

Function

Call (1.b) to generate one data point

Update the prior, and calculate the parameters of predictive distribution Repeat steps above until the posterior probability converges.

Output

Print the new data point and the current paramters for posterior and predictive distribution.

After probability converged, do the visualization

Ground truth function (from linear model generator)

Final predict result

At the time that have seen 10 data points

At the time that have seen 50 data points

Except ground truth, you have to draw those data points which you have seen before

Draw a black line to represent the mean of function at each point

Draw two red lines to represent the variance of function at each point

In other words, distance between red line and mean is <strong>ONE</strong> variance

Hint: Online learning

Sample input &amp; output (<strong><em>for reference only</em></strong>)

<ol>

 <li>b = 1, n = 4, a = 1, w = [1, 2, 3, 4]</li>

</ol>




<table width="627">

 <tbody>

  <tr>

   <td width="37">30313233343536373839404142434445464748495051525354555657585960616263646566676869707172737475767778</td>

   <td width="590">Predictive distribution ~ N(0.06869, 1.66008)————————————————-Add data point (-0.19330, 0.24507):Postirior mean:0.57609723130.2450231522-0.08018424530.0504992402Posterior variance:0.2867129751,   0.1311255325,  -0.0767580827,   0.04384885420.1311255325,   0.7892001707,   0.1242887609,  -0.0801412282-0.0767580827,   0.1242887609,   0.9176812972,   0.05415755400.0438488542,  -0.0801412282,   0.0541575540,   0.9642058389Predictive distribution ~ N(0.62305, 1.34848)————————————————-…————————————————-Add data point (-0.76990, -0.34768):Postirior mean:    0.91074966751.92654998853.11192971294.1312375189Posterior variance:0.0051883836,  -0.0004416700,  -0.0086000319,   0.0008247001-0.0004416700,   0.0401966605,   0.0012708906,  -0.0554822477-0.0086000319,   0.0012708906,   0.0265353911,  -0.00312058750.0008247001,  -0.0554822477,  -0.0031205875,   0.0937197255Predictive distribution ~ N(-0.61566, 1.00921)————————————————-Add data point (0.36500, 2.22705):Postirior mean:0.91074045831.92652250903.11194087404.1312734131Posterior variance:0.0051731092,  -0.0004872471,  -0.0085815201,   0.0008842340</td>

  </tr>

 </tbody>

</table>

<ol start="2">

 <li>b = 100, n = 4, a = 1, w = [1, 2, 3, 4]</li>

 <li>b = 1, n = 3, a = 3, w = [1, 2, 3]</li>

</ol>


