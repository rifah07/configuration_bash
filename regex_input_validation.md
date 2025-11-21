# Regex & Input Validation: Introduction and Questions

## Introduction to Regex and Input Validation

Regular Expressions (Regex) are powerful patterns used to match character combinations in strings. They are essential for validating user inputs, searching, and data parsing. Regex enables defining complex validation rules succinctly, making it widely used in form validation, data cleansing, and security checks.

Input validation ensures the data received conforms to expected formats—this is crucial for preventing errors and security vulnerabilities such as injection attacks.

Key features of Regex in validation:
- Pattern matching with literals, character classes, quantifiers, groups, and anchors
- Flags to control case sensitivity, multiline handling, etc.
- Use in both client-side and server-side validation
- Integration with many programming languages and tools

## Common Regex & Input Validation Questions and Answers

1. **What is a regular expression?**  
   A regex is a sequence of characters defining a search pattern, mainly used for text matching and validation.

2. **Why is input validation important?**  
   It ensures data correctness, prevents unexpected errors, and guards against malicious input like SQL injection or cross-site scripting.

3. **How do you match a pattern using regex?**  
   Use anchors (`^` for start, `$` for end) and character classes (`[0-9]`, `[A-Za-z]`) with quantifiers (`{3,5}`, `+`, `*`) to specify valid inputs.

4. **Give an example regex for validating an email.**  
```
^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+.[a-zA-Z]{2,}$
```

5. **How do you validate a phone number using regex?**  
Example for international format:  
```
^+\d{7,15}$
```

6. **What is the difference between greedy and lazy quantifiers?**  
Greedy quantifiers match as much as possible, lazy quantifiers match the least possible.  
Example: `a.*b` (greedy) vs `a.*?b` (lazy).

7. **How can regex be used for password validation?**  
Use positive lookaheads to enforce rules like minimum length, inclusion of uppercase, digits, and special characters:  
```
^(?=.[A-Z])(?=.\d)(?=.*\W).{8,}$
```

8. **What are some pitfalls of overusing regex?**  
Complex regex can be hard to read, maintain, and may cause performance issues or catastrophic backtracking.

9. **How do you handle invalid inputs gracefully?**  
Provide clear error messages, highlight input errors, and prevent form submission until validation passes.

10. **How do you test regex patterns?**  
 Use online tools like [Regex101](https://regex101.com/) or integrated development environment (IDE) regex testers.

---
