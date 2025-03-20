1. Sorting Employee Objects Using Lambda Expressions
This program defines an Employee class with attributes: name, age, and salary.
A list of employees is created and sorted using lambda expressions based on different criteria:
By Name → employees.sort((emp1, emp2) -> emp1.name.compareTo(emp2.name));
By Age → employees.sort((emp1, emp2) -> Integer.compare(emp1.age, emp2.age));
By Salary → employees.sort((emp1, emp2) -> Double.compare(emp1.salary, emp2.salary));
The sorted lists are printed after each sorting operation.
2. Filtering and Sorting Students Using Lambda and Streams
This program defines a Student class with name and marks.
A list of students is created and processed using streams and lambda expressions:
Filter students scoring above 75% → .filter(s -> s.marks > 75)
Sort in descending order → .sorted(Comparator.comparingDouble(s -> -s.marks))
Extract names → .map(s -> s.name)
Collect and display the result → .collect(Collectors.toList())
Finally, the names of students who scored above 75% are displayed.
