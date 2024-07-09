# Global Sequence Alignment

This repository contains implementations of the global sequence alignment algorithm for general English strings using dynamic programming and divide-and-conquer approaches. These algorithms ensure optimal and efficient string alignment, which is crucial for various applications like bioinformatics, text comparison, and more.

## Features

- **Dynamic Programming Approach**: Utilizes a dynamic programming matrix to store alignment scores, ensuring an optimal alignment by considering all possible alignments and their respective scores.
- **Divide and Conquer Strategy**: Enhances efficiency by breaking down the problem into smaller subproblems, solving each recursively, and combining the results. This approach reduces space complexity significantly.
- **Scoring System**: Implements a customizable scoring system for matches, mismatches, and gaps, allowing flexibility for different types of sequence data.
- **Traceback Mechanism**: Developed a traceback mechanism to reconstruct the optimal alignment path from the computed dynamic programming matrix.

## Files

- `dynamic_programming.cpp`: Contains the implementation of the global sequence alignment algorithm using the dynamic programming approach.
- `divide_and_conquer.cpp`: Contains the implementation of the global sequence alignment algorithm using the divide-and-conquer approach.
- `Report.pdf` : Contains the detailed analysis of thes dynamic programming and divide and conquer approach to sequence alignment

## How to Run

### Dynamic Programming Approach

1. Compile the code:
    ```sh
    g++ dynamic_programming.cpp -o dynamic_programming
    ```
2. Run the executable:
    ```sh
    ./dynamic_programming
    ```

### Divide and Conquer Approach

1. Compile the code:
    ```sh
    g++ divide_and_conquer.cpp -o divide_and_conquer
    ```
2. Run the executable:
    ```sh
    ./divide_and_conquer
    ```

## Example

### Input

```cpp
Sequences inputs[] = {
    {"correct", "corract"}, 
    {"fast", "fasting"}, 
    {"cat", "dog"}, 
    {"dog", "dig"}, 
    {"internet", "interest"}, 
    {"happiness", "happening"}, 
    {"computer", "commuter"}, 
    {"programming", "program"}, 
    {"transform", "transaction"}
};
```

### Output

Case 1 :-
- Sequence 1 : 'corr ect'
- Sequence 2 : 'corra ct'

Case 2 :-
- Sequence 1 : 'fast   '
- Sequence 2 : 'fasting'

Case 3 :-
- Sequence 1 : ' cat'
- Sequence 2 : 'd og'

Case 4 :-
- Sequence 1 : 'dog'
- Sequence 2 : 'dig'

Case 5 :-
- Sequence 1 : 'interne t'
- Sequence 2 : 'inter est'

Case 6 :-
- Sequence 1 : 'happ  iness'
- Sequence 2 : 'happenin  g'

Case 7 :-
- Sequence 1 : 'co mputer'
- Sequence 2 : 'comm uter'

Case 8 :-
- Sequence 1 : 'programming'
- Sequence 2 : 'progra m   '

Case 9 :-
- Sequence 1 : 'trans    form'
- Sequence 2 : 'transacti o n'
