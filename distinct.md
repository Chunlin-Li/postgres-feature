
# Distinct

```sql
SELECT *, test.id is distinct from t1.id FROM test , test t1;
+------+---------+------+---------+------------+
|   id |   value |   id |   value | ?column?   |
|------+---------+------+---------+------------|
|    2 |      20 |    2 |      20 | False      |
|    2 |      20 |    1 |      10 | True       |
|    1 |      10 |    2 |      20 | True       |
|    1 |      10 |    1 |      10 | False      |
+------+---------+------+---------+------------+

```