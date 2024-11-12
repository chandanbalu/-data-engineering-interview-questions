# SQL
+ [How can you retrieve the latest and oldest records for each name in a dataset and, for the oldest record, calculate the total of amounts for all records associated with that name?]
Given the following sample data:
ID	Name	created_on	Amount
A1	A	2023-04-01	10
A2	A	2023-04-02	10
A3	A	2023-04-03	10
A4	A	2023-04-04	10
A5	A	2023-04-05	10
A6	A	2023-04-06	10
B1	B	2023-04-01	20
B2	B	2023-04-02	20
B3	B	2023-04-03	20
B4	B	2023-04-04	20

The expected output should be:
ID	Name	created_on	Amount
A1	A	2023-04-01	60
A6	A	2023-04-06	10
B1	B	2023-04-01	80
B4	B	2023-04-04	20

What SQL query can I use to produce this result?