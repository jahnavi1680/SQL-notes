# SQL-notes
just some notes that I am making while practicing SQL


a new thing I learned today --- Window functions in MySQL

syntax: similar to aggregate;

sum(column) over(partition by other_column)

if you do an order by inside, its a rolling sum (dang)

more special things!!!

Row number, rank and dense_rank

---- wow we can give row numbers
syntax-- row_number() over()

---- ranks ---- rank() over(partition by column order by column)

************IMPORTANT***********
When using window function, we cannot use where clause conditioning the window columns (i.e. rank, sum or avg etc)

