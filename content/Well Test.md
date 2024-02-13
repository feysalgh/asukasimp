### Role of Oil Well Tests and Information in Petroleum Industry
Oil well test analysis is a branch of reservoir engineering. Information obtained from flow and pressure transient tests about in situ reservoir conditions are important to determining the productive capacity of a reservoir.
In general, oil well test analysis is conducted to meet the following objectives:
- To evaluate well condition and reservoir characterization
- To obtain reservoir parameters for reservoir description
- To determine whether all the drilled length of oil well is also a producing zone
- To estimate skin factor or drilling- and completion-related damage to an oil well. Based upon the magnitude of the damage, a decision regarding well stimulation can be made.

This chapter deals with the basic equations for flow of liquid through porous media along with solutions of interest for various boundary conditions
and reservoir geometry. These solutions are required in the design and interpretation of flow and pressure tests.

## Fundamentals of Reservoir Oil Flow Analysis
#### Basic Fluid Flow Equations in Oil Reservoir
##### Steady-State Flow Equations and Their Practical Applications
 The steady-state flow equations are based on the following assumptions:
 1. Thickness is uniform, and permeability is constant
 2. Fluid is incompressible
 3. Flow across any circumference is a constant.
###### Ideal Steady-State Flow Equation - Radial Flow

$$ q_o =\frac{0.00708k_{imp}h(p_e-p_{wf}-\Delta p_{skin})}{\mu_o B_o \ln(r_e/r_w)} $$
###### pseudo-steady-state equation - Radial flow
$$p-p_{wf}=\frac{141.2q_o\mu_oB_o}{kh}(\ln(\frac{r}{r_w'})-0.75)$$
in which:
$$r_w'=r_we^{-s}$$
a. damaged well $s>0$
b. stimulated well $s<0$

###### Time to Reach Pseudo-Steady State
Dimensionless time $t_D$, which is used to define various flow regimes, is given as:
$$t_D=\frac{0.00264kt}{\phi\mu c_{t}r_w^2}$$
where:
$k$ = permeability, mD
$t$ = time, hr
$\phi$ = porosity in fraction
$\mu_o$ = oil viscosity, cp
$c_{ti}$ = initial total compressibility, psi^-1
$r_w$ = wellbore radius, ft


## Pressure Drawdown Testing Testing Techniques for Oil Wells
A pressure drawdown test is simply a series of bottom-hole pressure measurements made during a period of flow at a constant production rate. transient flow condition prevails to a value of real time approximately equal to:
$$t\approx\frac{\phi\mu_o r_e^2}{0.00264k}$$
Semi-steady-state conditions are established at a time value of:
$$t\approx \frac{\phi \mu_o cr_e^2}{0.00088k}$$
### Pressure-Time History for Constant-Rate Drawdown Test
This figure shows the flow history of an oil well and can be classified into three periods for analysis:
- Transient or early flow period is usually used to analyze flow characteristics 
- Late transient periods is more completed
- Semi-steady-state flow periods is used in reservoir limit tests. 
![[Pasted image 20231105185154.png]]

##### Transient Analysis - Infinite-Acting Reservoir
An ideal constant-rate drawdown test in an infinite-acting reservoir is modeled by the logarithmic approximation to the Ei-function solution:
$$p_{wf}=p_i-141.2\frac{q_o\mu_o B_o}{kh}\big[p_D(t_D)+s\big]$$
Assuming initially the reservoir at initial pressure, Pi, the dimensionless pressure at the well ($r_D =1$) is given as:
$$p_D=0.5\big[\ln(t_D)+0.80907\big]$$
After the wellbore storage effects have diminished and $t_D/r_D^2 >100$ dimensionless time is given by:
$$t_D=\frac{0.002673kt}{\phi\mu_o c_t r_w^2}$$
Combining and rearranging these equations, we get a familiar form of the pressure drawdown equation:
$$p_{wf}=p_i-\frac{162.6q_o\mu_o B_o}{kh}\bigg[\log t+\log\bigg(\frac{k}{\phi \mu_o c_t r_w^2}\bigg)-3.23 + 0.869s\bigg]$$
This equation describes a straight line with intercept and slope term together and it may be written as:
$$p_{wf}=m\log t+p_{1hr}$$
A plot of flowing bottom-hole pressure data versus the logarithm of flowing time should be a straight line with slope $m$ and intercept $p_{1hr}$. Semilog straight line does appear after wellbore damage and storage effects have diminished. The slope of the semilog straight line may be given by:
$$m=-\frac{162.6q_o\mu_oB_o}{kh}$$
![[Pasted image 20231105190720.png]]
The intercept at $\log t=0$, which occurs at $t=1$, is also determined from:
$$p_{1h}=p_i+m\bigg[\log\bigg(\frac{k}{\phi\mu_o B_o c_t r_w^2}\bigg)-3.23+0.869s\bigg]$$
The skin factor is estimated from a rearranging form of the last equation:
$$s=1.151\bigg[\frac{p_i-p_{1hr}}{m}-\log\bigg(\frac{k}{\phi\mu_oc_tr_w^2}\bigg)+3.23\bigg]$$
The beginning time of the semilog straight line may be estimated from log-log plot of $[\log(p_i-p_{wf})]$ versus $\log t$ (the bellow figure); when the slope of the plot is one cycle in $\Delta p$ per cycle in $t$, wellbore storage dominates and test data give no information about the formation. The wellbore storage coefficient may be estimated from the unit-slope straight line using the following equation: 
$$C=\frac{q_o B_o}{24}.\frac{\Delta t}{\Delta p}$$
where $\Delta t$ and $\Delta p$ are the calues read from a point on the log-log unit slope straight line.
![[Pasted image 20231105192748.png]]

##### Late Transient Analysis - Bounded (Developed) Reservoirs
Pressure behavior at constant rate in a bounded reservoir can by:
$$\log(p_{wf}-\hat p)=\log(b_1)-(\beta_1)t$$
From this we see that a plot of $log(p_{wf}-\hat p)$  versus t should be linear with slope magnitude:
$$\beta_1=\frac{0.00168k}{\phi \mu_ocr_e}$$
and intercept
$$b_1 =118.6\frac{q_o\mu_oB_o}{kh}$$
the plot of $\log(p_{wf}-\hat p)$ versus $t$ will be linear provided the value of $\hat p$ is known. usually it is not. this means that trial and error plot must be made using assumed $\hat p$ values. That value which yields the best straight line on the $\log(p_{wf}-\hat p)$ versus $t$ t is chosen as the correct $\hat p$ value.  A schematic late transient drawdown analysis plot is shown in the Figure.
![[Pasted image 20231105211153.png]]
After determining the correct $\hat p$ value, $kh$ can be estimated from the intercept value $b$ by:
$$kh=\frac{118.6 q_o \mu_o B_o}{b}$$
The pore volume (drainage volume) of the well:
$$V_p=0.1115\frac{q_o B_o}{\beta_1 b_1 c_t}$$
$$r_e=\bigg[\frac{A\times43,560}{\pi}\bigg]^{0.5}$$
The skin factor can be found from
$$s = 0.84\big[\frac{\bar p-\hat p}{b_1}\big]-\ln(\frac{r_e}{r_w})+0.75$$
$$(\Delta p)_{skin}=\frac{b_1s}{0.84}$$

## Pressure Buildup Analysis Techniques for Oil Wells
Pressure buildup testing is the most familiar transient well-testing technique, which has been used extensively in the petroleum industry. Basically, the test is conducted by producing a well at constant rate for some time, shutting the well in (usually at the surface), allowing the pressure to build up in the wellbore, and recording the down-hole pressure in the wellbore as a function of time.
### Ideal pressure buildup test
In an ideal situation, we assume that the test is conducted in an infinite acting reservoir in which no boundary effects are felt during the entire flow and later shut-in period. The reservoir is homogeneous and containing in slightly compressible, single-phase fluid with uniform properties so that the Ei function and its logarithmic approximation apply. Horner's approximation is applicable.

If a well is shut-in after it has produced at rate $q$ for time $t_p$ and bottom-hole pressure $p_{ws}$ is recorded at time $\Delta t$, then plot of $p_{ws}$ versus $\log((t_p+\Delta t)/\Delta t)$ will give a straight line, which is represented by the following equation:
$$p_{ws}=p_i-\frac{162.6q_o\mu_oB_o}{kh}\log\bigg[\frac{t_p+\Delta t}{\Delta t}\bigg]$$
$$m=\frac{162.6q_o\mu_oB_o}{kh}$$
$$k=\frac{162.6q_o\mu_oB_o}{mh}$$
and the skin factor is:
$$s=1.151\bigg[\frac{p_{1hr}-p_{ws(\Delta t=0)}}{m}-\log\bigg(\frac{k}{\phi\mu_oc_tr_w^2}\bigg)+3.23\bigg]$$
