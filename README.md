# Background
This is an independent student research project I conducted in the course "Workshop: society" at the university of St. Gallen. It uses all four waves of the Asian Barometer Survey, conducted by the College of Social Sciences, National Taiwan University Hu Fu Center for East Asia Democratic Studies. The data was kindly provided to me by its respective owners and will not be shared here.


# How to reproduce this study
In order to be able to run the analysis, you first need to request access to the first four waves of the ABS survey for the PRC: http://asianbarometer.org/data/data-release

1. Create a folder "data_ABS" in the directory that the .Rproj and .r file are stored.

2. Place the .sav files of the four waves of surveys in the "data_ABS" folder. Name them "abs_PRC_wave1.sav", "abs_PRC_wave2.sav", "abs_PRC_wave3.sav", "abs_PRC_wave4.sav". Do not use subfolders.

3. To finally reproduce the code, first open up the .Rproj file, then open up the .r file and executive it.

# Results
This study investigates two questions: 

- How does political trust in central government change between 2002 and 2016 in the PRC?
- Do self-expression values, by themselves or incombination with political interest, exert a negative impact on trust in central government in the PRC?

In answering the first question, this study confirms other research in that it finds a consistently decreasing average level of political trust. To obtain these averages, survey responses ranging from "a great deal of trust", "quite a lot of trust", not very much trust", "none at all", were coded from 4 to 1.

In answering the second question, this study finds no significant effect of self-expression values on political trust, neither alone nor in combination with political interest.

Attached below are a plot addressing the first question and a regression table addressing the second.



![average trust over time](plots/trend.png)




<table style="text-align:center"><caption><strong>OLS model, dependent variable: political trust in national government</strong></caption>
<tr><td colspan="5" style="border-bottom: 1px solid black"></td></tr><tr><td style="text-align:left"></td><td>(1)</td><td>(2)</td><td>(3)</td><td>(4)</td></tr>
<tr><td colspan="5" style="border-bottom: 1px solid black"></td></tr><tr><td style="text-align:left">Age</td><td>0.002<sup>***</sup> (0.001)</td><td>0.002<sup>**</sup> (0.001)</td><td>0.002<sup>**</sup> (0.001)</td><td>0.002<sup>**</sup> (0.001)</td></tr>
<tr><td style="text-align:left">Female</td><td>-0.076<sup>***</sup> (0.023)</td><td>-0.068<sup>***</sup> (0.023)</td><td>-0.069<sup>***</sup> (0.023)</td><td>-0.068<sup>***</sup> (0.023)</td></tr>
<tr><td style="text-align:left">Formal education years</td><td>0.005 (0.003)</td><td>0.004 (0.003)</td><td>0.004 (0.003)</td><td>0.004 (0.003)</td></tr>
<tr><td style="text-align:left">Is unemployed</td><td>-0.038 (0.027)</td><td>-0.037 (0.027)</td><td>-0.037 (0.027)</td><td>-0.037 (0.027)</td></tr>
<tr><td style="text-align:left">Rural residence</td><td>0.084<sup>***</sup> (0.026)</td><td>0.081<sup>***</sup> (0.026)</td><td>0.081<sup>***</sup> (0.026)</td><td>0.082<sup>***</sup> (0.026)</td></tr>
<tr><td style="text-align:left">Economic performance</td><td>0.058<sup>***</sup> (0.013)</td><td>0.055<sup>***</sup> (0.013)</td><td>0.055<sup>***</sup> (0.013)</td><td>0.055<sup>***</sup> (0.013)</td></tr>
<tr><td style="text-align:left">Healthcare</td><td>-0.015 (0.016)</td><td>-0.017 (0.016)</td><td>-0.017 (0.016)</td><td>-0.017 (0.016)</td></tr>
<tr><td style="text-align:left">Corruption</td><td>-0.145<sup>***</sup> (0.024)</td><td>-0.147<sup>***</sup> (0.024)</td><td>-0.147<sup>***</sup> (0.024)</td><td>-0.147<sup>***</sup> (0.024)</td></tr>
<tr><td style="text-align:left">Unfairness of income distribution</td><td>-0.045<sup>***</sup> (0.016)</td><td>-0.045<sup>***</sup> (0.016)</td><td>-0.045<sup>***</sup> (0.016)</td><td>-0.044<sup>***</sup> (0.016)</td></tr>
<tr><td style="text-align:left">Patriotism</td><td>0.177<sup>***</sup> (0.018)</td><td>0.176<sup>***</sup> (0.018)</td><td>0.177<sup>***</sup> (0.018)</td><td>0.176<sup>***</sup> (0.018)</td></tr>
<tr><td style="text-align:left">Respect for authority</td><td>0.036<sup>**</sup> (0.017)</td><td>0.039<sup>**</sup> (0.017)</td><td>0.039<sup>**</sup> (0.017)</td><td>0.039<sup>**</sup> (0.017)</td></tr>
<tr><td style="text-align:left">Allocentric self-interest</td><td>0.127<sup>***</sup> (0.018)</td><td>0.123<sup>***</sup> (0.019)</td><td>0.123<sup>***</sup> (0.019)</td><td>0.123<sup>***</sup> (0.019)</td></tr>
<tr><td style="text-align:left">Internet use</td><td>-0.010<sup>*</sup> (0.005)</td><td>-0.011<sup>**</sup> (0.005)</td><td>-0.010<sup>**</sup> (0.005)</td><td>-0.011<sup>**</sup> (0.005)</td></tr>
<tr><td style="text-align:left">Self-expression values index</td><td>0.018 (0.026)</td><td>0.016 (0.026)</td><td></td><td>0.062 (0.074)</td></tr>
<tr><td style="text-align:left">Political interest</td><td></td><td>0.027<sup>*</sup> (0.014)</td><td></td><td>0.071 (0.069)</td></tr>
<tr><td style="text-align:left">SE values * political interest</td><td></td><td></td><td>0.010<sup>*</sup> (0.005)</td><td>-0.020 (0.030)</td></tr>
<tr><td style="text-align:left">Constant</td><td>2.341<sup>***</sup> (0.162)</td><td>2.326<sup>***</sup> (0.163)</td><td>2.368<sup>***</sup> (0.154)</td><td>2.221<sup>***</sup> (0.229)</td></tr>
<tr><td colspan="5" style="border-bottom: 1px solid black"></td></tr><tr><td style="text-align:left">Observations</td><td>2,199</td><td>2,183</td><td>2,183</td><td>2,183</td></tr>
<tr><td style="text-align:left">R<sup>2</sup></td><td>0.222</td><td>0.224</td><td>0.224</td><td>0.224</td></tr>
<tr><td style="text-align:left">Adjusted R<sup>2</sup></td><td>0.217</td><td>0.219</td><td>0.219</td><td>0.218</td></tr>
<tr><td style="text-align:left">Residual Std. Error</td><td>0.519 (df = 2184)</td><td>0.518 (df = 2167)</td><td>0.518 (df = 2168)</td><td>0.518 (df = 2166)</td></tr>
<tr><td style="text-align:left">F Statistic</td><td>44.569<sup>***</sup> (df = 14; 2184)</td><td>41.682<sup>***</sup> (df = 15; 2167)</td><td>44.616<sup>***</sup> (df = 14; 2168)</td><td>39.094<sup>***</sup> (df = 16; 2166)</td></tr>
<tr><td colspan="5" style="border-bottom: 1px solid black"></td></tr><tr><td style="text-align:left"><em>Note:</em></td><td colspan="4" style="text-align:right"><sup>*</sup>p<0.1; <sup>**</sup>p<0.05; <sup>***</sup>p<0.01</td></tr>
</table>

