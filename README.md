# Runoff Voting

This project implements a **runoff voting system** in C, based on ranked-choice voting. The program allows multiple candidates to run in an election and multiple voters to rank the candidates in order of preference. If no candidate wins a majority, the candidate with the fewest votes is eliminated, and votes are redistributed until a winner is found or a tie is detected.

---

## Features

- Accepts any number of candidates (up to 9).
- Accepts any number of voters (up to 100).
- Allows voters to rank candidates.
- Automatically tabulates votes in rounds.
- Eliminates candidates with the fewest votes.
- Detects ties.
- Declares the winner once a candidate has a majority.

---

## Usage

Compile the program using:

```bash
make runoff
```

Run it by passing candidate names as command-line arguments:

```bash
./runoff Alice Bob Charlie
```

You'll then be prompted to enter the number of voters, and each voter's ranked choices.

---

## Example

```
$ ./runoff Alice Bob Charlie
Number of voters: 3
Rank 1: Alice
Rank 2: Charlie
Rank 3: Bob

Rank 1: Bob
Rank 2: Charlie
Rank 3: Alice

Rank 1: Charlie
Rank 2: Alice
Rank 3: Bob

Charlie
```

---

## File Structure

- `runoff.c` – Main program implementing the runoff voting logic.
- `README.md` – This file.

---

## Concepts Covered

✅ Arrays  
✅ Structs  
✅ Nested loops  
✅ Logical thinking  
✅ Elimination algorithm  
✅ Working with strings

---

## Credit

Built as part of the [CS50](https://cs50.harvard.edu/) course by Harvard University.

---