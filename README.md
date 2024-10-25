README for AST Rule Evaluator
Overview
This program evaluates a set of logical rules based on user-provided data, utilizing an Abstract Syntax Tree (AST) structure to represent the rules. It can handle logical operations (AND, OR) and various comparison operations on numeric and string data.

Features
Dynamic Rule Creation: Users can input rules using a string format, which are parsed and transformed into an AST.
User Input: The program collects user data for evaluation against the rules.
Evaluation of Rules: Each rule can be evaluated individually, as well as combined to see if any of them hold true for the given data.
Debugging Information: Debug prints provide insights into the evaluation process.
Installation
To run this program, ensure you have Python installed (Python 3.6 or higher recommended). No additional packages are required.

Usage
Run the program: Execute the script in a Python environment.

Input data: You will be prompted to enter the following data:

Age (integer)
Department (string)
Salary (integer)
Experience (integer)
Rules: The program contains two pre-defined rules:

Rule 1: ((age > 30 AND department = 'Sales') OR (age < 25 AND department = 'Marketing')) AND (salary > 50000 OR experience > 5)
Rule 2: ((age > 30 AND department = 'Marketing')) AND (salary > 20000 OR experience > 5)
Results: After input, the program evaluates each rule and outputs the results.

Code Structure
Node Class: Represents an AST node, handling logical operations and operand evaluation.
create_rule Function: Parses a rule string and constructs an AST.
combine_rules Function: Combines multiple rules into a single AST using the OR operator.
evaluate_rule Function: Evaluates the constructed AST against the user-provided data.
get_user_input Function: Collects user input for age, department, salary, and experience.
Example Output
After entering your data, you will see outputs similar to:

mathematica
Copy code
Rule 1 Evaluation Result: True
Rule 2 Evaluation Result: False
Combined Rule Evaluation Result: True
Notes
The rules are defined in a specific string format, with logical operators (AND, OR) and comparison operators (>, <, >=, <=, =).
String comparisons are case-insensitive.
Ensure proper formatting of strings in the rules (e.g., strings should be enclosed in single quotes).
Contributing
Feel free to contribute to this project by forking the repository and submitting a pull request.
