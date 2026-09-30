[← Back to Module 2](../README.md)

# Module 2 — Exercises

Do each part right after its matching notebook/script. **Attempt every
exercise yourself before opening the matching file in `solutions/`.** Per
the [AI usage policy](../../../docs/ai-usage-policy.md), it's fine to use
an AI assistant to review your finished attempt — not to write it for you.

## Part 1 — Variables and Types
*(after `01_variables_and_types`)*

1. Create variables for a product's `name` (str), `price` (float), and
   `in_stock` (bool). Print a sentence describing the product using an
   f-string, formatting the price to 2 decimal places.
2. Given `sentence = "  Data Science is Fun  "`, write code that prints the
   sentence with whitespace stripped, in uppercase, with "Fun" replaced by
   "Powerful".
3. Given two numbers `a = 29` and `b = 4`, print the result of every
   arithmetic operator (`+ - * / // % **`) with a label, without
   copy-pasting from the notebook — write it from memory.
4. A user enters their age as text: `age_text = "27"`. Convert it to an
   `int` and print whether they are 18 or older.

*Solution:* [solutions/01_variables_and_types_solution.py](solutions/01_variables_and_types_solution.py)

## Part 2 — Data Structures
*(after `02_data_structures`)*

1. Given `prices = [12.50, 8.00, 25.00, 8.00, 3.75]`, write code to: remove
   one `8.00`, add `15.00`, sort ascending, then print the sum and the
   average.
2. Write a list comprehension that returns only the prices above 10 from
   the list in Q1.
3. Create a dictionary representing a book (`title`, `author`, `year`,
   `genres` as a list). Add a new key `in_library` set to `True`. Print
   every key and value using a loop.
4. Given `tags_a = {"python", "beginner", "course"}` and
   `tags_b = {"python", "advanced", "project"}`, print their union,
   intersection, and the tags only in `tags_a`.
5. Given a list of transaction dicts (reuse the shape from the notebook),
   write code that returns a **list of unique categories** using a set.

*Solution:* [solutions/02_data_structures_solution.py](solutions/02_data_structures_solution.py)

## Part 3 — Control Flow
*(after `03_control_flow`)*

1. Write a function-free script that classifies a `score` variable (0-100)
   into `"F"`, `"D"`, `"C"`, `"B"`, or `"A"` using `if`/`elif`/`else`.
2. Using a `for` loop and `range()`, print all multiples of 3 between 1 and
   50.
3. Using a `while` loop, keep doubling a starting value of `1` until it
   exceeds `1000`, printing each value along the way. Count how many
   doublings it took.
4. Given a list of transactions (description/amount/category dicts), write
   a loop that prints only the transactions in the `"food"` category,
   using `continue` to skip the rest.
5. Write a loop that stops (`break`) as soon as it finds the first
   transaction over `$100`, and prints which one it was.

*Solution:* [solutions/03_control_flow_solution.py](solutions/03_control_flow_solution.py)

## Part 4 — Functions and Modules
*(after `04_functions_and_modules`)*

1. Write a function `average(numbers)` that returns the average of a list
   of numbers. It should return `0` (not crash) for an empty list.
2. Write a function `is_palindrome(text)` that returns `True` if `text`
   reads the same forwards and backwards, ignoring case and spaces (e.g.
   `"Never Odd or Even"` → `True`).
3. Write a function `apply_discount(price, percent=10)` that returns the
   price after applying a percentage discount, with `percent` defaulting
   to 10.
4. Write two functions: `celsius_to_fahrenheit(c)` and
   `fahrenheit_to_celsius(f)`. Use one to check the other round-trips
   correctly for at least 3 values.
5. Using the `random` module, write a function `roll_dice(sides=6)` that
   returns a random integer from 1 to `sides`.

*Solution:* [solutions/04_functions_and_modules_solution.py](solutions/04_functions_and_modules_solution.py)

## Part 5 — Files, JSON, CSV, Error Handling
*(after `05_files_json_csv`)*

1. Write a function `save_notes(path, notes)` that writes a list of
   strings to a text file, one per line.
2. Write a function `load_json_safe(path)` that loads a JSON file and
   returns `{}` (not a crash) if the file doesn't exist or isn't valid
   JSON — reuse the `try/except` pattern from the notebook.
3. Create a small CSV of at least 5 fictional transactions
   (`description,amount,category`), then write code that reads it back and
   prints the total amount **per category** (a dict of `{category: total}`).
4. Deliberately trigger and catch a `KeyError` by accessing a dictionary
   key that doesn't exist, using `try/except`, and print a friendly message
   instead of letting the program crash.

*Solution:* [solutions/05_files_json_csv_solution.py](solutions/05_files_json_csv_solution.py)

## Part 6 — OOP, Debugging, Testing
*(after `06_oop_and_error_handling`)*

1. Add a `to_dict()` method to a `Transaction`-like class that returns a
   plain dict of its fields — useful for saving to JSON.
2. Write a `Budget` class with a `limit` (float) and a list of
   `Transaction`s. Add a method `is_over_budget()` that returns `True` if
   the total of its transactions exceeds `limit`.
3. Deliberately write a small function with a bug (e.g. an off-by-one
   error in a loop), run it, read the traceback (or the wrong output) from
   the bottom up, and fix it. Write one sentence describing what the bug
   was.
4. Write two `assert`-based tests for your `Budget` class from Q2: one
   where it's under budget, one where it's over.

*Solution:* [solutions/06_oop_and_error_handling_solution.py](solutions/06_oop_and_error_handling_solution.py)

## When you're done with all six parts

Move on to the module's capstone:
[project-personal-finance-tracker/](../project-personal-finance-tracker/README.md).
