# SQL
+ ## SQL Query to Retrieve Latest and Oldest Records with Aggregated Amounts

### Problem Description

Given a dataset with records for different names, we need to:

1. Retrieve the latest and oldest records for each name.
2. For the oldest record of each name, calculate the total of `Amount` values for all records associated with that name.

#### Input Data Example

| ID  | Name | created_on | Amount |
|-----|------|------------|--------|
| A1  | A    | 2023-04-01 | 10     |
| A2  | A    | 2023-04-02 | 10     |
| A3  | A    | 2023-04-03 | 10     |
| A4  | A    | 2023-04-04 | 10     |
| A5  | A    | 2023-04-05 | 10     |
| A6  | A    | 2023-04-06 | 10     |
| B1  | B    | 2023-04-01 | 20     |
| B2  | B    | 2023-04-02 | 20     |
| B3  | B    | 2023-04-03 | 20     |
| B4  | B    | 2023-04-04 | 20     |

#### Expected Output

| ID  | Name | created_on | Amount |
|-----|------|------------|--------|
| A1  | A    | 2023-04-01 | 60     |
| A6  | A    | 2023-04-06 | 10     |
| B1  | B    | 2023-04-01 | 80     |
| B4  | B    | 2023-04-04 | 20     |

In this output:
- For each name, the oldest record has the `Amount` field updated to the total of all `Amount` values for that name.
- The latest record retains its original `Amount` value.