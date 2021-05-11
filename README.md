### CRITIC-Weighting
Coding: UTF-8

Author: Victor Xu, Randal Jin

Time: 2021/5/11

E-mail: 

viktor.p.xu@yandex.ru

RandalJin@163.com

Description: If you are interested in empirically economic research,
CRITIC weighting will be a useful tool to construct a new variable.
(To finish the school paper, we coded it to test our skills, and hopefully it will be of use to you.)


### Usage Sample


<table>
	<tr>
	    <th>Upper Variable</th>
	    <th>Lower Variable</th>
	</tr >
	<tr >
	    <td rowspan="3">A Casual Econ Index</td>
	    <td>GDP</td>
	</tr>
	<tr>
	    <td>Inflation</td>
	</tr>
	<tr>
	    <td>Employment</td>
	</tr>


para = {'Econ Index': ['GDP', 'Inflation', 'Employment']}


f = 'C:/Users/ThinkPad/Desktop/data.xlsx'


df = pd.read_excel(f)


df = critic(df, para, std=True)
