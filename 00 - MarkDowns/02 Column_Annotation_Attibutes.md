> @Column annotation attributes
```java
    @Column(
        name = "emp_name",        // Custom column name
        length = 100,             // Maximum length of the column (for String types)
        nullable = false,        // Column cannot be null
        unique = true,           // Values in this column must be unique
        insertable = true,       // Include column in INSERT statements (default is true)
        updatable = true,        // Include column in UPDATE statements (default is true)
        columnDefinition = "VARCHAR(100) DEFAULT 'Unknown'"  // Custom SQL column definition
    )
    private String name;

    @Column(
        name = "emp_salary",     // Custom column name
        precision = 10,          // Precision of the column (total number of digits)
        scale = 2,               // Scale of the column (number of digits after the decimal point)
        nullable = false         // Column cannot be null
    )
    private BigDecimal salary;
///

> @Id annotation include @Column annotation inside it so no need to explicitly apply that again