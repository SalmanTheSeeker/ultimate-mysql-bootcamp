# ENUM Data Type:
ENUM stands for enumeration, and it allows you to specify a list of possible values for a column. Only one value from the list can be assigned to the column.
```sql
column_name ENUM(value1, value2, value3, ...)
```

```sql
CREATE TABLE enum_example (
    color ENUM('Red', 'Green', 'Blue')
);
```
```
-- Inserting values
INSERT INTO enum_example (color) VALUES ('Red'), ('Green'), ('Blue');

-- Querying data
SELECT * FROM enum_example;
```
![Enum datatypes](https://github.com/Techwiz-Laraib/ultimate-mysql-bootcamp/assets/159939710/33b344bb-b642-49d1-a7e4-2007cbc06656)


# SET Data Type:
SET is similar to ENUM, but it allows you to select multiple values from a predefined list. Values are stored as a set, and each value is separated by commas

```sql
column_name SET(value1, value2, value3, ...)
```

```sql
CREATE TABLE set_example (
    toppings SET('Cheese', 'Pepperoni', 'Mushrooms', 'Onions', 'Olives')
);
```
```sql
-- Inserting values
INSERT INTO set_example (toppings) VALUES ('Cheese, Pepperoni'), ('Mushrooms, Onions'), ('Cheese, Olives');

-- Querying data
SELECT * FROM set_example;
```
In both cases, you define the possible values for the column within parentheses after the data type declaration. When inserting data,
you provide values within single quotes, separated by commas if necessary.

![set datatypes](https://github.com/Techwiz-Laraib/ultimate-mysql-bootcamp/assets/159939710/d98b9d46-b450-474e-b30b-9161452cfb02)




