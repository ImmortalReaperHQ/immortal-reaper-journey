# Project 001: Reaper Expense Tracker

**Date:** 12 October 2026  
**Developer:** Immortal Reaper  
**Language:** C  
**Status:** Code review and corrections prepared; testing pending

## Today's Objective

Build and review my first C project, a simple command-line expense tracker.

## What I Worked On

- Created the initial expense tracker in C.
- Implemented options to add income, add expenses, view the balance, and exit.
- Reviewed the code to identify logical and formatting errors.
- Prepared corrections for the identified issues.

## Bugs Identified and Corrections Prepared

### 1. Income calculation

**Problem:** The income total was updated using the wrong expression.

**Correction:**

```c
income += amount;
```

**Lesson:** Update the variable that represents the total being tracked.

### 2. Insufficient balance validation

**Problem:** The expense validation condition was reversed.

**Correction:**

```c
amount > income - expense
```

**Lesson:** A program must reject an expense when it exceeds the available balance.

### 3. Currency formatting

**Problem:** The income display used an unsuitable floating-point format.

**Correction:**

```c
printf("Total Income  : Rs. %.2f\n", income);
```

**Lesson:** `%.2f` displays two digits after the decimal point.

### 4. Invalid menu options

**Problem:** The menu did not handle unsupported choices.

**Correction:** Added a `default` case to the `switch` statement.

### 5. Output readability

**Problem:** Some messages needed newline characters and spelling corrections.

**Correction:** Improved the output formatting and corrected the project name.

## Testing

Testing has not yet been completed or confirmed.

- [ ] Compile the program with warnings enabled.
- [ ] Add ₹1,000 income and check the total.
- [ ] Add a ₹250 expense and check the ₹750 balance.
- [ ] Attempt a ₹800 expense and verify it is rejected.
- [ ] Test zero and invalid menu input.
- [ ] Verify that the exit option works.

## What I Learned

- How small logic errors can change program behavior.
- Why conditional operators matter.
- How to format decimal values.
- Why input validation and testing are important.
- How to review code and document corrections.

## Current Limitations

- Data disappears when the program closes.
- Transaction history is not saved.
- Invalid numeric input terminates the program.

## Next Steps

- [ ] Upload the corrected `main.c` to the project repository.
- [ ] Compile and run the program.
- [ ] Complete the tests and record actual results.
- [ ] Improve invalid-input handling.

**Project:** Reaper Expense Tracker  
**Motto:** BUILD. EARN. EVOLVE.

https://github.com/ImmortalReaperHQ/reaper-expense-tracker
