df1 = data.frame(CustId = c(1:6), Product = c(rep("TV", 3), rep("Radio", 3)))
df2 = data.frame(CustId = c(2, 4, 6), State = c(rep("Texas", 2), rep("NYC", 1)))
df1 #left table
df2 #right table
For the above given data frames and tables perform the following operations:
Return only the rows in which the left table have match
       Ans.       Left_table <- merge(df1, df2 , by = "CustId")
                      Left_table
        2. Return all rows from both tables, join records from the left which have matching keys in the right          table.
Ans.

          total <- merge(df1, df2, all = TRUE)
          total

