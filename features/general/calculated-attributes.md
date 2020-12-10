# Calculated Attributes
User Calculated Attributes are user-defined objects, which extend the system entities.
Calculated attributes are defined like formulas.
When the value of a calculated attribute is requested, it is calculated "on the fly", in real time.

> [!NOTE]
> Calculated attribute formulas are compiled to native executable format.
> Their calculation speed is very similar to the speed of the system defined calculated attributes.

## Example - Get default payment term days

Suppose, that in a Sales Order, we want to display the customers default payment term (in days).
In the Sales Order, we can define the following Calculated Attribute:

| No | Operation | Param1 | Param2 | Param3 |
|----|-----------|--------|--------|--------|
| 10 | GETREF | REF:Customer | ATTRIB:DefaultPaymentTermDays |

Explanation:

- GETREF - gets information from a related entity. The related entity is specified in Param1. The desired information is specified in Param2.
- Line number 10 is the only line in the calculated attribute
- The return value is the value of the attribute DefaultPaymentTermDays in the Customer entity.

## Example - Complex filter and summation

The following calculated attribute sums all sales order lines, whose product:

- has a user data attribute, called "CustPropPrj", equal to '500'
- has a Name, containing the word 'Tool'


| No | Operation | Param1 | Param2 | Param3 |
|----|-----------|--------|--------|--------|
| 10 | SUM | EXP:20 | ATTRIB:LineAmount |
| 20 | FILTER | CHILD:Lines | EXP:30 |
| 30 | IN | ATTRIB:Product | EXP:40 |
| 40 | FILTER | QUERY:Gen_Products | EXP:50 |
| 50 | AND | EXP:60 | EXP:70 |
| 60 | EQUALS | ATTRIB:CustPropPrj | CONST:500 |
| 70 | LIKE | ATTRIB:Name | CONST:'Tool' |

Explanation:

- Line 10: Iterates through the data set, specified on Line 20 (EXP:20), then SUMs the attribute LineAmount.
- Line 20: Filters the Lines subset with the filter, specified in Line 30 (EXP:30).
- Line 30: Creates a filter, which will be satisfied only by products, specified in the query on Line 40 (EXP:40).
- Line 40: Creates a query, which filters the products with the condition, specified on Line 50.
- Line 50: Specifies that the condition is comprised of two conditions, linked with AND.
- Line 60: Specifies that the first condition is the value of an attribute, called CustPropPrj should be 500.
- Line 70: Specifies that the second condition is that the Name of the product should contain 'Tool'.

This example demonstrates, that Calculated Attributes can calculate very complicated formulas, query the database, get related values, etc.
