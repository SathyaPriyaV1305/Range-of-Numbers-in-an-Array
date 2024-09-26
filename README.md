// C Program to Find the Range of Numbers in an Array

#include <stdio.h>

int main()
{

    // Initialize an array
    int arr[] = { 23, 12, 45, 20, 90, 89, 95, 32, 65, 19 };

    // Finding size of an array
    int n = sizeof(arr) / sizeof(arr[0]);

    // Intialize the first element of the array as both
    // maximum and minimum value
    int min = arr[0];
    int max = arr[0];

    // Find the maximum and minimum value in the array
    for (int i = 1; i < n; i++) {
        if (max < arr[i])
            max = arr[i];

        if (min > arr[i])
            min = arr[i];
    }
    // Calculating the range of an array
    int range = max - min;

    // Printing the range of an array
    printf("The range of the array is %d:", range);

    return 0;
}
# Range-of-Numbers-in-an-Array
