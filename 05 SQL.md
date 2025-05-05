<details>

<summary>
#1 Explain normalization
</summary>

<br/>

> A database design technique to remove/avoid redundant data

</details>

<details>

<summary>
#2 How to implement normalization?
</summary>

<br/>

> By splitting tables and using the reference data in the master table.

</details>

<details>

<summary>
#3 Explain denormalization
</summary>

<br/>

>  database design technique to improve search performance
>
> How to achieve this? We merge tables

</details>

<details>

<summary>
#4 OLTP vs OLAP
</summary>

<br/>

> OLTP/Online Transaction Processing - transactions; uses normalization
>
> OLAP/Online Analytical Processing - analytics; uses denormalization
>
> OLTP -> ETL -> OLAP

</details>

<details>

<summary>
#5 Explain 1st, 2nd and 3rd normal form
</summary>

<br/>

> 1st: a table is in first normal form when the columns have atomic values or does not have repeating groups.
>
>> Example: don’t use full name as a single column, create first, middle and last name columns
>>
> 2nd: first normal form should be satisfied. All non-key columns should be fully dependent on the primary key.
>
> 3rd: all 1st and 2nd normal form should be satisfied. No transient dependency should be present.

</details>

<details>

<summary>
#6 Primary Key vs Unique Key
</summary>

<br/>

> Similarity: ensures we're not allowing duplicates
>
> Differences
>
>> In unique key, null is allowed
>>
>> Unique keys can be multiple in a table but only one primary key

</details>

<details>

<summary>
#7 Char vs Varchar
</summary>

<br/>

> Char is fixed length while varchar is dynamic

</details>

<details>

<summary>
#8 Char vs Nchar
</summary>

<br/>

> If you want to store english characters then use char
>
> If you want to use multi language use Nchar (unicode)

</details>

<details>

<summary>
#9 What's the size of Char vs Nchar
</summary>

<br/>

> 1 character in char = 1 byte
>
> 1 character in nchar = 2 bytes

</details>

<details>

<summary>
#10 What's the use of index
</summary>

<br/>

> Indexes increases search performance

</details>

<details>

<summary>
#11 How does it make search faster?
</summary>

<br/>

> Creates balance tree structure to reach the data quick
>
> Example: encyclopedia are grouped by letter; this way search is easier

</details>

<details>

<summary>
#12 What are two types of indexes?
</summary>

<br/>

> Clustered index
>
> Non-clustered index

</details>

<details>

<summary>
#13 Clustered vs Non-clustered Index
</summary>

<br/>

> Clustered index - leaf node is pointing to the data directly
>
> Non-clustered index - uses clustered index to locate the data

</details>

<details>

<summary>
#14 Function vs Stored Procedure
</summary>

<br/>

> Goal: functions are for computing values while stored procs act as a mini batch program.
>
> Impact: functions will not make any permanent changes to the environment while stored procs can change the environment.
>
> Actions allowed: functions only allow selects while stored procs allows CRUD
>
> I/O: function should have one input with a return value while stored procs can have zero parameter and can return one or more outputs.
>
> Execution: functions can be called from select/where/call from other stored proc. Stored procs cannot be executed from a select/where or from other functions.

</details>

<details>

<summary>
#15 What are triggers and why do you need them?
</summary>

<br/>

> Triggers are logics which can be executed when events like insert, update, delete, etc. happens

</details>

<details>

<summary>
#16 What are types of triggers?
</summary>

<br/>

> After trigger: triggers after the action has been executed
>
> Instead of trigger: replaces the action that was supposed to be executed
</details>

<details>

<summary>
#18 What is the identity column in SQL?
</summary>

<br/>

> Identity helps to define auto-increment column

</details>

<details>

<summary>
#19 Explain transactions and how to implement them?
</summary>

<br/>

> Transactions help us to treat a series of activities as one logical unit
>
> Either everything is successful or everything rollbacks
>
> Usage: enclose with begin tran & commit tran

</details>

<details>

<summary>
#20 What are inner joins?
</summary>

<br/>

> Inner join matches records from both tables
>
> Example: select * from table1 inner join table2 on table1.uniquekey = table2.primarykey

</details>

<details>

<summary>
#21 What are left joins?
</summary>

<br/>

> All data from left table are selected plus matching records from the right table
>
> Example: select * from table1 left join table2 on table1.uniquekey = table2.primarykey

</details>

<details>

<summary>
#22 What are right joins?
</summary>

<br/>

> All data from right table are selected plus matching records from the left table
>
> Example: select * from table1 right join table2 on table1.uniquekey = table2.primarykey

</details>

<details>

<summary>
#23 What are full outer joins?
</summary>

<br/>

> All matching and unmatching records from both left and right tables are selected
>
> Example: select * from table1 full outer join table2 on table1.uniquekey = table2.primarykey

</details>

<details>

<summary>
#24 Explain cross join
</summary>

<br/>

> Combines each row from one table with every row from another table creating cartesian product of the two tables.
>
> Example: select * from table1 cross join table2

</details>

<details>

<summary>
#25 Why do we need a UNION?
</summary>

<br/>

> Unions help to combine two result sets and excludes duplicates

</details>

<details>

<summary>
#26 Union vs Union All
</summary>

<br/>

> Both help combine two result sets. Difference is union excludes duplicates while union all includes it.

</details>

<details>

<summary>
#27 Can we have unequal columns in a union?
</summary>

<br/>

> No, union requires an equal number of expressions

</details>

<details>

<summary>
#28 Can columns have different data types in union?
</summary>

<br/>

> No

</details>

<details>

<summary>
#29 Which aggregate function have you used?
</summary>

<br/>

> Count
>
> Sum
>
> AVG or average
>
> Max
>
> Min

</details>

<details>

<summary>
#30 When to use group by?
</summary>

<br/>

> Group by helps you to convert rows to summary rows using common values
>
> Example: select ProductName, Sum(ProductAmount) from tbl group by ProductName

</details>

<details>

<summary>
#31 Can we select column which is not part of groupby?
</summary>

<br/>

> No, it should be part of aggregate or group by

</details>

<details>

<summary>
#32 What is having clause?
</summary>

<br/>

> Having clause helps to filter group by data
>
> Example: select ProductName, Sum(ProductAmount) from tbl group by ProductName having ProductName='Shoes'

</details>

<details>

<summary>
#33 Having clause vs where clause
</summary>

<br/>

> Where is applied in the row level (select statement) while having is applied in the group by result
>
> Having can use aggregate while where cannot

</details>

<details>

<summary>
#34 How can we sort records?
</summary>

<br/>

> By using order by clause

</details>

<details>

<summary>
#35 What is the default sort?
</summary>

<br/>

> Ascending

</details>

<details>

<summary>
#36 How can we remove duplicates?
</summary>

<br/>

> By using distinct keyword

</details>

<details>

<summary>
#37 Select the first top x records
</summary>

<br/>

> By using top x keyword

</details>

<details>

<summary>
#38 How to handle nulls?
</summary>

<br/>

> By using ISNULL function
>
> Isnull(column, replacementValue)

</details>

<details>

<summary>
#39 What is the use of wild cards?
</summary>

<br/>

> Wild cards help in pattern matching
>
> Use like keyword and % or _
>
> Example: select * from table where column like 'a%'

</details>

<details>

<summary>
#40 What is the use of alias?
</summary>

<br/>

> Use as keyword
>
> Helps to give different display names to original column names
>
> Especially helpful when merging two tables with the same column name

</details>

<details>

<summary>
#41 How to write a case statement?
</summary>

<br/>

> Example: Select ProductAmount, CASE WHEN ProductAmount < 100 THEN 'Less than 100' ELSE 'More than 100' END AS ProductAmount From table

</details>

<details>

<summary>
#42 What is self-reference tables?
</summary>

<br/>

> Are tables who have primary and foreign key in the same table.

</details>

<details>

<summary>
#43 What is self-join?
</summary>

<br/>

> When you use joins with the same table

</details>

<details>

<summary>
#44 Explain between clause
</summary>

<br/>

> Used to select a range
>
> Example: Select * from table where ProductAmount between 0 and 100

</details>

<details>

<summary>
#45 Explain Subquery
</summary>

<br/>

> Query inside a query

</details>

