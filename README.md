# EPAIAssignment13
EPAiAssignment13

# Goal 1
Create a lazy iterator that will return a named tuple of the data in each row. The data types should be appropriate - i.e. if the column is a date, you should be storing dates in the named tuple, if the field is an integer, then it should be stored as an integer, etc.

# Goal 2
Calculate the number of violations by car make.

Note:
Try to use lazy evaluation as much as possible - it may not always be possible though! That's OK, as long as it's kept to a minimum.

No Test Cases

# Functions
* cast(data_type, value): Function to cast the value to the appropriate datatype. it takes data_types and value as argument and return typecast value.
* cast_row(data_type, value): Function which takes one row and sends the elements one by one for casting. Returns a list of casted elements 
* get_data(file): This function to yield one row at a time (leaving out first line).An iterator function (the function becomes an iterator because of the yield in the function) which reads lazily (line by line from the file) and calls the function for casting. Once the elements are casted to proper datatypes, it is returned back.
* gen_iters(): An lazy iterator
* ctr_dict(): Function to count the violations. Uses a dictionary to count the number of violations by each brand car. This would include data even if the name of the car is blank or violation description is blank
* get_voilations_by_car_make(make_name): Return the number of voilations by a car make
