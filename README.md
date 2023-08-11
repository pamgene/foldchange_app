#  Fold Change App

##### Description

The `foldchange_app` is an application that calculates the ratio (fold change) between the Test and the Control condition.
It requires 
- log-transformed data
- a pairing factor (e.g. Replicate or pair)

Example input design:

\begin{table}[]
\begin{tabular}{lllll}
Sample name1 & Replicate & Supergroup & Test Condition & pair  \\
C-1          & 1         & Sgroup1    & Control        & pair1 \\
T1-1         & 1         & Sgroup1    & T1             & pair1 \\
T2-1         & 1         & Sgroup1    & T2             & pair1 \\
T3-1         & 1         & Sgroup1    & T3             & pair1 \\
C-2          & 2         & Sgroup1    & Control        & pair2 \\
T1-2         & 2         & Sgroup1    & T1             & pair2 \\
T2-2         & 2         & Sgroup1    & T2             & pair2 \\
T3-2         & 2         & Sgroup1    & T3             & pair2
\end{tabular}
\end{table}



##### Details

The `foldchange_app` calculates fold change by subtracting the values of the Test Condition from the Control for each pair within each supergroup. 
It returns the mean fold change among pairs for each supergroup.