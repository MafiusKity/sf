# sf
A function in R to propagate error for any expression whit variables associeted whit error

This fuction aply the formula for propagate error at all variables whit error:

$\sigma_{f}=\sqrt{\sum^{variables}(\frac{\partial f}{\partial variable}\sigma_{variable})^2}$

## Usage
To use this fuction, just run in your R enviroment:

```
source("path/sf.R") #path is the path containing this script
sf(expression,...) #... = ("variable",variable_value,variable_error)*n_variables
```
The arguments after expression (...) can be reapeat any times for diferents variables in this order ("variable1",variable1_value,variable1_error,"variable2",variable2_value,variable2_error,...). 

## Limitations
- The function dosent works whit matix but works whit vactors or lists, except to argument expression;
- The function dosent works whit differential equations or fuctions such as sum;
