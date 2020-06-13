

Cleanup steps
* Outside of script
    * Identify variables not in data dictionaries
    * Identify variables with lots of nulls, or which could be captured by more general variables
    * Identify data type
    * Identify representatives for classes of missing columns
* Automated cleanup
    * Exclude columns
    * Switch all NaN values to NaN
    * Identify numerics, fill in NaN with mean
        * Might want to impute better, if time permits
    * Convert non-numerics to categoricals
    * Make NaN dummy column for representatives
    
** Don't forget to add in the customer columns later! **