# SQL-Auto-Doc

Generate Markdown-documentation from your database. Example:

# data.users

Employees who have software licenses.

| ID        | Name   | Type(Length)   | Nullable   | Default   | Example                      | Comment                                   |
| --------- | ------ | -------------- | ---------- | --------- | ---------------------------- | ----------------------------------------- |
| 455672671 | joined | datetime2(8)   | true       | 0         | 2017-01-01                   | Date when the employee joined our company |
| 455672671 | age    | int(4)         | true       | 0         | 42                           | The age of the employee                   |
| 455672671 | id     | bigint(8)      | false      | 0         | 5                            | Primary Key, technical                    |
| 455672671 | name   | nvarchar(800)  | false      | 0         | “Peter Peterson”             | Name of the employee                      |
| 455672671 | email  | nvarchar(800)  | false      | 0         | “peter.peterson@company.com” | E-mail address of the employee            |


# data.software

Software bought for or by the company

| ID        | Name      | Type(Length)   | Nullable   | Default   | Example          | Comment                                    |
| --------- | --------- | -------------- | ---------- | --------- | ---------------- | ------------------------------------------ |
| 487672785 | installed | datetime2(8)   | true       | 0         | 2016-04-16       | Date the software was first installed      |
| 487672785 | id        | int(4)         | false      | 0         | 5                | Primary Key, technical                     |
| 487672785 | name      | nvarchar(800)  | true       | 0         | “Office 2016”    | Name of the software                       |
| 487672785 | creator   | nvarchar(800)  | true       | 0         | “Microsoft”      | Creator behind the software                |
| 487672785 | website   | nvarchar(800)  | true       | 0         | “www.office.com” | Website of the software product or creator |




### Aim: Maven- or Flyway-Plugin

### Similar Projects

- https://github.com/vokal/pg-table-markdown (for PostgreSQL)
- https://stackoverflow.com/questions/186392/how-do-you-document-your-database-structure
- Redgate SQL Doc (http://www.red-gate.com/products/sql-development/sql-doc/)
- ApexSQL Doc (https://www.apexsql.com/sql_tools_doc.aspx)
- SchemaSpy (http://schemaspy.sourceforge.net)
