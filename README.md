# fdaCOVID2
Contains Rdata to perform analysis from [_'Contrasting pre-vaccine COVID-19 waves in Italy through Functional Data Analysis'_](https://arxiv.org/abs/2307.09820).

---

### DATA DESCRIPTION

The file `fdaCOVID2git.Rdata` contains 2 data structures: `covariates` and `fd_data`


---

`covariates` is a data frame whose columns are the 12 scalar variables investigated in the paper for the 107 Italian provinces

--- 

`fd_list` is a list containing all the information regarding the functional variables investigated in the paper. 
It includes 3 different sub-list: 
 * `wave0`
   * raw data for a period of 485 days 


 * `wave1`  
   * `raw` data for the period of 150 days corresponding to the first wave 
   * `smoothed` curves for all the functional variables 
   * `lags`: difference in days from March 9th, 2020, to the maximum of the mortality curves 
   * `shifted`: 
     * `shifts`: translations applied to functional variables 
     * `curves`: translated curves 
     * `cl_k2`, `cl_k3`: clusters obtained with a functional hierarchical algorithms for 2 and 3 groups, respectively


 * `wave2`  
   * `raw` data for the period of 150 days corresponding to the second wave 
   * `smoothed` curves for all the functional variables 
   * `lags`: difference in days from November 4th, 2020, to the maximum of the mortality curves 
   * `shifted`: 
     * `shifts`: translations applied to functional variables 
     * `curves`: translated curves 
     * `cl_k2`, `cl_k3`: clusters obtained with a functional hierarchical algorithms for 2 and 3 groups, respectively
