# BITPE
******************************************
***************Author*********************
******************************************

Johannes König
Research Fellow - DIW Berlin/SOEP
Email: jkoenig@diw.de
Website: https://sites.google.com/view/johanneskoenig/home

************************************************
***************Introduction*********************
************************************************

This ReadMe file explains where one can find the code that generates
each table, figure and calculation in the text in the codebase
in order of appearance in the paper.

Overall, the code can be understood in the following way:

There are several subfolders that refer to the different datasets used in
the paper:
	1.For the Heathcote et al. (2017) replication: ~\HSV and ~\CBO
	2.For the direct estimation of progressivity based on the PSID: ~\direct_prog
	3.For the Kaas et al. (2021) replication: ~\KKPS
	4.For calculations based on the estimates: ~\impact_calculation


********************************************
***************Software*********************
********************************************

This project required the use of several software packages.

1. Stata Version 17

2. Wolfram Mathematica Version 11.3

3 Matlab Version R2018	  

4. Microsoft Excel 

Data handling and most calculation are performed in Stata.
Mathematica and Matlab are only required for the calculations in ~\impact_calculation.


*****************************************************
***************Data Availability*********************
*****************************************************

I provide the final prepared data files for calculations in the paper and
not the raw data files. Below I describe how to access the raw data.


1. PSID:
For the direct estimation of progressivity I do not provide the
full set of PSID data files for replication, but only the output past running NBER's TAXSIM.
You will have to download your own copy of the PSID data if you wish to fully replicate the dataset.
The PSID can be downloaded here: https://simba.isr.umich.edu/data/data.aspx
Access to TAXSIM and the legacy versions can be found here: https://taxsim.nber.org/

2. CBO data:
The tabular data for the CBO dataset is fully provided in the replication files.

3. SOEP:
The SOEP is freely available only to the research community. The data have to be
ordered using the form on this website: https://www.diw.de/en/diw_01.c.601584.en/data_access.html
The version of the data I used is:
Socio-Economic Panel (SOEP),data for years 1984-2014, version 31


*************************************************************************
***************Code Locations for Figures and Tables*********************
*************************************************************************


***************Tables*********************

Table 2 : 
		
  		~\HSV\do\regs.do

Table 3: 
		~\HSV\do\log_lin_test.do

Table 4:
		~\CBO\do\02_tax_approx.do

Table 5:
		~\KKPS\rep\regs.do
		~\KKPS\rep\log_lin_test.do

Table 6: 	
  		~\impact_calculation\frisch.xlsx

Table B1:
		~\HSV\do\regs_by_y.do

Table B2:
		~\HSV\do\regs_by_t.do

Table B3:
		~\HSV\do\regs_pos_tax.do
		~\KKPS\rep\pos_tax.do

Table D4:
		this is synthetic data

Table F5:
		~\impact_calculation\get_vars.wls


*****************Figures******************

Figure 1:
		 ~\HSV\do\regs.do

Figure 2
		 ~\HSV\do\binplots.do

Figure 3:
		 ~\direct_prog\prog_do\02_direct_prog.do

Figure 4:
		 ~\KKPS\rep\binplots.do

Figure 5:
		 ~\impact_calculation\imp_calc.do

Figure 6:
		 ~\impact_calculation\imp_calc.do		 

************Calculations in Text***************

AMTR calculation:
		~\HSV\do\calc_trate.do

Optimal progressivity Exercises:
		~\impact_calculation\get_vars.wls
		~\impact_calculation\HSV_impact.m
		~\impact_calculation\HSV_imp.nb

