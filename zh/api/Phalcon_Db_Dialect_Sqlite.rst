Class **Phalcon\\Db\\Dialect\\Sqlite**
======================================

*extends* :doc:`Phalcon\\Db\\Dialect <Phalcon_Db_Dialect>`

*implements* :doc:`Phalcon\\Db\\DialectInterface <Phalcon_Db_DialectInterface>`

Generates database specific SQL for the Sqlite RBDM


Methods
---------

public  **getColumnDefinition** (:doc:`Phalcon\\Db\\ColumnInterface <Phalcon_Db_ColumnInterface>` $column)

Gets the column name in Sqlite



public *string*  **addColumn** (*string* $tableName, *string* $schemaName, :doc:`Phalcon\\Db\\ColumnInterface <Phalcon_Db_ColumnInterface>` $column)

Generates SQL to add a column to a table



public *string*  **modifyColumn** (*string* $tableName, *string* $schemaName, :doc:`Phalcon\\Db\\ColumnInterface <Phalcon_Db_ColumnInterface>` $column)

Generates SQL to modify a column in a table



public *string*  **dropColumn** (*string* $tableName, *string* $schemaName, *string* $columnName)

Generates SQL to delete a column from a table



public *string*  **addIndex** (*string* $tableName, *string* $schemaName, :doc:`Phalcon\\Db\\IndexInterface <Phalcon_Db_IndexInterface>` $index)

Generates SQL to add an index to a table



public *string*  **dropIndex** (*string* $tableName, *string* $schemaName, *string* $indexName)

Generates SQL to delete an index from a table



public *string*  **addPrimaryKey** (*string* $tableName, *string* $schemaName, :doc:`Phalcon\\Db\\IndexInterface <Phalcon_Db_IndexInterface>` $index)

Generates SQL to add the primary key to a table



public *string*  **dropPrimaryKey** (*string* $tableName, *string* $schemaName)

Generates SQL to delete primary key from a table



public *string*  **addForeignKey** (*string* $tableName, *string* $schemaName, :doc:`Phalcon\\Db\\Reference <Phalcon_Db_Reference>` $reference)

Generates SQL to add an index to a table



public *string*  **dropForeignKey** (*string* $tableName, *string* $schemaName, *string* $referenceName)

Generates SQL to delete a foreign key from a table



protected *array*  **_getTableOptions** ()

Generates SQL to add the table creation options



public *string*  **createTable** (*string* $tableName, *string* $schemaName, *array* $definition)

Generates SQL to create a table in PostgreSQL



public *boolean*  **dropTable** (*string* $tableName, *string* $schemaName, *boolean* $ifExists)

Generates SQL to drop a table



public *string*  **tableExists** (*string* $tableName, *string* $schemaName)

Generates SQL checking for the existence of a schema.table <code>echo $dialect->tableExists("posts", "blog") <code>echo $dialect->tableExists("posts")



public *string*  **describeColumns** (*string* $table, *string* $schema)

Generates a SQL describing a table <code>print_r($dialect->describeColumns("posts") ?>



public *array*  **listTables** (*string* $schemaName)

List all tables on database <code>print_r($dialect->listTables("blog") ?>



public *string*  **describeIndexes** (*string* $table, *string* $schema)

Generates SQL to query indexes on a table



public *string*  **describeIndex** (*string* $indexName)

Generates SQL to query indexes detail on a table



public *string*  **describeReferences** (*string* $table, *string* $schema)

Generates SQL to query foreign keys on a table



public *string*  **tableOptions** (*string* $table, *string* $schema)

Generates the SQL to describe the table creation options



public *string*  **limit** (*string* $sqlQuery, *int* $number) inherited from Phalcon\\Db\\Dialect

Generates the SQL for LIMIT clause



public *string*  **forUpdate** (*string* $sqlQuery) inherited from Phalcon\\Db\\Dialect

Returns a SQL modified with a FOR UPDATE clause



public *string*  **sharedLock** (*string* $sqlQuery) inherited from Phalcon\\Db\\Dialect

Returns a SQL modified with a LOCK IN SHARE MODE clause



public *string*  **getColumnList** (*array* $columnList) inherited from Phalcon\\Db\\Dialect

Gets a list of columns



public *string*  **getSqlExpression** (*array* $expression, *string* $escapeChar) inherited from Phalcon\\Db\\Dialect

Transform an intermediate representation for a expression into a database system valid expression



public *string*  **getSqlTable** (*unknown* $table, *string* $escapeChar) inherited from Phalcon\\Db\\Dialect

Transform an intermediate representation for a schema/table into a database system valid expression



public *string*  **select** (*array* $definition) inherited from Phalcon\\Db\\Dialect

Builds a SELECT statement



