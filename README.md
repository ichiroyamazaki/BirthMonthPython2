# BirthMonthPython2

**BirthMonthPython2** is a simple Python console application that compares the birth months of two groups of classmates and checks whether the user's birth month matches any month entered by either group.

The project demonstrates Python set operations, user input, string formatting, and conditional statements.

## Features

- Collects three birth months for Group 1.
- Collects three birth months for Group 2.
- Stores birth months in Python sets to avoid duplicate entries.
- Converts entered month names to capitalized form.
- Displays the birth months of both groups.
- Calculates the union of the two sets.
- Calculates the intersection of the two sets.
- Calculates the difference between the two sets.
- Checks whether the user's birth month matches a month entered by a classmate.

## Requirements

- Python 3
- A Python-compatible IDE or code editor, or a terminal

## Project Structure

```text
BirthMonthPython2/
├── birth_month.py
├── README.md
└── pom.xml
```

## How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/ichiroyamazaki/BirthMonthPython2.git
```

### 2. Open the Project Directory

```bash
cd BirthMonthPython2
```

### 3. Run the Program

```bash
python birth_month.py
```

Depending on your system, you may need to use:

```bash
python3 birth_month.py
```

## How It Works

1. The program asks for three birth months for Group 1.
2. It asks for three birth months for Group 2.
3. The entered months are capitalized and stored in sets.
4. The program displays both groups.
5. It calculates the union, intersection, and difference of the sets.
6. The user enters their own birth month.
7. The program checks whether that month appears in either group and displays a matching or non-matching message.

## Understanding the Set Operations

Let `set1` represent Group 1 and `set2` represent Group 2.

| Operation | Python syntax | Meaning |
|---|---|---|
| Union | `set1 \| set2` | All unique months from both groups |
| Intersection | `set1 & set2` | Months shared by both groups |
| Difference | `set1 - set2` | Months in Group 1 that are not in Group 2 |

## Example

```text
Enter birth month 1: January
Enter birth month 2: March
Enter birth month 3: June
Enter birth month 1: March
Enter birth month 2: August
Enter birth month 3: December

Group 1: {'January', 'March', 'June'}
Group 2: {'March', 'August', 'December'}

Enter your birth month: March
Union: {'January', 'March', 'June', 'August', 'December'}
Intersection: {'March'}
Difference: {'January', 'June'}
You have the same birth month with one of your classmates
```

*Note: Python sets are unordered, so the order of months displayed may vary.*

## Concepts Demonstrated

- **Sets:** Store unique birth month values.
- **Union:** Combines the unique elements of two sets.
- **Intersection:** Identifies elements shared by both sets.
- **Difference:** Finds elements that belong to one set but not the other.
- **String methods:** Uses `.capitalize()` to normalize month-name capitalization.
- **Conditional statements:** Checks whether the user's month matches a month in either group.
- **Console input and output:** Uses `input()` and `print()` to interact with the user.

## Limitations

- The program does not validate whether the entered month is a real calendar month.
- Each group accepts three inputs, but duplicate entries are stored only once because sets contain unique elements.
- The final birth-month comparison is case-sensitive because the user's input is checked against the sets without capitalization.
- The program does not store results after it closes.

## Author

**Ichiro Yamazaki**

## License

No license is currently specified in the repository. Check the repository for licensing information before redistributing or modifying the project.
