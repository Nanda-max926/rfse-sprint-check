# Time and Space Complexity - rfSE Sprint1

Analyze each C program to determine its time and space complexity.

## Easy Programs

1. Find the maximum value in an array of integers.

```c
#include <stdio.h>
int main() {
    int n, arr[100];
    scanf("%d", &n);
    for(int i=0; i<n; i++) scanf("%d", &arr[i]);
    int max = arr[0];
    for(int i=1; i<n; i++) if(arr[i] > max) max = arr[i];
    printf("%d\n", max);
    return 0;
}
```

2. Check if a number is even or odd.

```c
#include <stdio.h>
int main() {
    int num;
    scanf("%d", &num);
    if(num % 2 == 0) printf("Even\n");
    else printf("Odd\n");
    return 0;
}
```

3. Sum all elements in an array.

```c
#include <stdio.h>
int main() {
    int n, arr[100];
    scanf("%d", &n);
    for(int i=0; i<n; i++) scanf("%d", &arr[i]);
    int sum = 0;
    for(int i=0; i<n; i++) sum += arr[i];
    printf("%d\n", sum);
    return 0;
}
```

4. Print numbers from 1 to n.

```c
#include <stdio.h>
int main() {
    int n;
    scanf("%d", &n);
    for(int i=1; i<=n; i++) printf("%d ", i);
    printf("\n");
    return 0;
}
```

5. Access the middle element of an array (assume even length).

```c
#include <stdio.h>
int main() {
    int n, arr[100];
    scanf("%d", &n);
    for(int i=0; i<n; i++) scanf("%d", &arr[i]);
    printf("%d\n", arr[n/2]);
    return 0;
}
```

6. Swap two integers without a temporary variable.

```c
#include <stdio.h>
int main() {
    int a, b;
    scanf("%d %d", &a, &b);
    a = a + b;
    b = a - b;
    a = a - b;
    printf("%d %d\n", a, b);
    return 0;
}
```

7. Count the number of vowels in a string.

```c
#include <stdio.h>
#include <string.h>
int main() {
    char str[100];
    scanf("%s", str);
    int count = 0;
    for(int i=0; str[i]; i++) {
        char c = tolower(str[i]);
        if(c=='a' || c=='e' || c=='i' || c=='o' || c=='u') count++;
    }
    printf("%d\n", count);
    return 0;
}
```

8. Find the length of a string without using strlen.

```c
#include <stdio.h>
int main() {
    char str[100];
    scanf("%s", str);
    int len = 0;
    while(str[len]) len++;
    printf("%d\n", len);
    return 0;
}
```

9. Check if a number is prime.

```c
#include <stdio.h>
int main() {
    int n;
    scanf("%d", &n);
    int isPrime = 1;
    if(n < 2) isPrime = 0;
    for(int i=2; i*i<=n; i++) {
        if(n % i == 0) isPrime = 0;
    }
    printf("%s\n", isPrime ? "Prime" : "Not Prime");
    return 0;
}
```

10. Calculate factorial using a loop.

```c
#include <stdio.h>
int main() {
    int n;
    scanf("%d", &n);
    long long fact = 1;
    for(int i=1; i<=n; i++) fact *= i;
    printf("%lld\n", fact);
    return 0;
}
```

## Moderate Programs

1. Binary search on a sorted array.

```c
#include <stdio.h>
int main() {
    int n, key, arr[100];
    scanf("%d %d", &n, &key);
    for(int i=0; i<n; i++) scanf("%d", &arr[i]);
    int low=0, high=n-1, found=-1;
    while(low <= high) {
        int mid = low + (high-low)/2;
        if(arr[mid] == key) { found = mid; break; }
        else if(arr[mid] < key) low = mid+1;
        else high = mid-1;
    }
    printf("%d\n", found);
    return 0;
}
```

2. Merge two sorted arrays into one.

```c
#include <stdio.h>
int main() {
    int n, m, arr1[100], arr2[100], res[200];
    scanf("%d %d", &n, &m);
    for(int i=0; i<n; i++) scanf("%d", &arr1[i]);
    for(int i=0; i<m; i++) scanf("%d", &arr2[i]);
    int i=0, j=0, k=0;
    while(i<n && j<m) {
        if(arr1[i] <= arr2[j]) res[k++] = arr1[i++];
        else res[k++] = arr2[j++];
    }
    while(i<n) res[k++] = arr1[i++];
    while(j<m) res[k++] = arr2[j++];
    for(int p=0; p<k; p++) printf("%d ", res[p]);
    printf("\n");
    return 0;
}
```

3. Sort an array using bubble sort.

```c
#include <stdio.h>
int main() {
    int n, arr[100];
    scanf("%d", &n);
    for(int i=0; i<n; i++) scanf("%d", &arr[i]);
    for(int i=0; i<n-1; i++) {
        for(int j=0; j<n-i-1; j++) {
            if(arr[j] > arr[j+1]) {
                int temp = arr[j];
                arr[j] = arr[j+1];
                arr[j+1] = temp;
            }
        }
    }
    for(int i=0; i<n; i++) printf("%d ", arr[i]);
    printf("\n");
    return 0;
}
```
