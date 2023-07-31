#  Fold Change App

##### Description

`foldchange_app` is an application that calculates the ratio (fold change) between the Test and the Control condition.
It requires 
- log-transformed data
- pairing factor which has to be different from the observation (it cannot be barcode, array) 

##### Details

The `foldchange_app` calculates fold change by subtracting the values of the Test Condition from the Control for each pair within each supergroup. 
It returns the mean fold change among pairs for each supergroup.