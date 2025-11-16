# Ex7 Removal of Nodes with a Specific Value from a Linked List
## DATE:
## AIM:
To write a java  program that removes all nodes from a linked list whose value matches a given integer (val) and returns the new head of the modified linked list.

## Algorithm

1. Start
2. Read the size of the array `n`
3. Read array elements `arr[0..n-1]`
4. Read the position `pos` to delete
5. If `pos < 0` or`pos >= n` then

   * Print `"Invalid position!"`
   * Stop
6. Else

   * For `i = pos` to `n-2`
   * `arr[i] = arr[i+1]`  // shift elements left
   * Reduce `n` by 1 (`n = n - 1`)
7. Print the updated array `arr[0..n-1]`
8. End


## Program:
```
/*
program that removes all nodes from a linked list whose value matches a given integer (val) and returns the new head of the modified linked list.
Developed by:Nalini P
RegisterNumber:212223220063
*/

import java.util.Scanner;

public class DeleteAtPosition {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int n = scanner.nextInt();
        int[] array = new int[n];
        for (int i = 0; i < n; i++) {
            array[i] = scanner.nextInt();
        }
       
        int pos = scanner.nextInt();
        if (pos < 0 || pos >= n) {
            System.out.println("Invalid position");
        }
        else {
            for (int i = pos; i < n - 1; i++) {
                array[i] = array[i + 1]; }
                n--;
                for (int i = 0; i < n; i++) {
        System.out.print(array[i] + " ");
    }
}

         
           
        scanner.close();
    }
}
```
## Output:

<img width="708" height="253" alt="image" src="https://github.com/user-attachments/assets/53339a36-554d-4a1c-9cb0-3a54726862ee" />


## Result:
The java program successfully removes all nodes with the specified value (val) from the linked list and returns the new head.
