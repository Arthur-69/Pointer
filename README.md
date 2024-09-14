Pointer Assignments

Assignment 1: Basics of Pointers

Code Explanation:
1. We declare an integer variable x initialized to 10.
2. A pointer ptr is declared, which stores the address of x using the address-of operator (&).
3. We print the address of x using both &x and ptr, which will output the same memory address.
4. The value of x is modified by dereferencing the pointer (*ptr), and the new value is printed.

Assignment 2: Pointer Arithmetic

Code Explanation:
1. We declare an array of integers arr[] and a pointer p pointing to the start of the array.
2. The pointer is used to traverse the array and print each element using pointer arithmetic (*(p + i)).
3. Each element of the array is modified by multiplying it by 2, and the modified array is printed both using the array name and pointer arithmetic.

Assignment 3: Pointers and Functions

Code Explanation:
1. The swap() function takes two integer pointers and swaps the values they point to.
2. In main(), we declare two integers x and y and pass their addresses to swap().
3. The values of x and y are printed before and after the swap.

Assignment 4: Pointers to Pointers

Code Explanation:
1. We declare an integer x, a pointer p that points to x, and a pointer pp that points to p.
2. The value of x is printed using both *p and **pp.

Processes Assignments

Assignment 1: Basic Process Creation with fork()

Code Explanation:
1. The fork() function is used to create a child process.
2. In the child process, we print the child's PID using getpid(), while in the parent process, we print the parent’s PID.

Assignment 2: Using wait() and waitpid()

Code Explanation:
1. The wait() function is used to make the parent process wait for the first child to finish.
2. A second child is created using fork(), and waitpid() is used to wait for the second child. The exit status of both children is printed using the status code from wait() and waitpid().

Assignment 3: Understanding atexit()

Code Explanation:
1. Two functions are registered using atexit(). These functions are executed automatically when the program terminates.
2. The exit() function is called, and the order of function execution is observed.

Assignment 4: Fork and Exit Status

Code Explanation:
1. Two child processes are created using fork(). Each child returns a different exit code using exit().
2. The parent uses waitpid() to wait for each child and prints the exit status.

Assignment 5: Handling Zombie Processes

Code Explanation:
1. A child process is created, and the parent does not call wait(), resulting in a zombie process.
2. The program is modified to include wait() in the parent, preventing the child from becoming a zombie.
