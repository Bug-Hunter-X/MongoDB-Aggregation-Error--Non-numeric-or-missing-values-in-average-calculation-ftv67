# MongoDB Aggregation Error: Handling Non-Numeric Values in Average Calculation

This repository demonstrates a common error in MongoDB aggregation pipelines when calculating averages.  If the field used for averaging contains missing values (null or undefined) or non-numeric values (strings, objects), the aggregation pipeline will fail.

The `bug.js` file contains the erroneous aggregation pipeline. The `bugSolution.js` file provides a corrected version using the `$ifNull` and `$toDouble` operators to handle potential errors.