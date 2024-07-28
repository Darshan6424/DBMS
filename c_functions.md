
# Basic Arithmetic Operations in C

This document provides separate C programs for basic arithmetic operations using different configurations of functions.

## 1. Function with Return Type and with Arguments

### Addition

```c
#include <stdio.h>

int add(int a, int b);

int main() {
    int a = 10, b = 5;
    printf("Addition: %d\n", add(a, b));
    return 0;
}

int add(int a, int b) {
    return a + b;
}
```

### Subtraction

```c
#include <stdio.h>

int subtract(int a, int b);

int main() {
    int a = 10, b = 5;
    printf("Subtraction: %d\n", subtract(a, b));
    return 0;
}

int subtract(int a, int b) {
    return a - b;
}
```

### Multiplication

```c
#include <stdio.h>

int multiply(int a, int b);

int main() {
    int a = 10, b = 5;
    printf("Multiplication: %d\n", multiply(a, b));
    return 0;
}

int multiply(int a, int b) {
    return a * b;
}
```

### Quotient

```c
#include <stdio.h>

int quotient(int a, int b);

int main() {
    int a = 10, b = 5;
    printf("Quotient: %d\n", quotient(a, b));
    return 0;
}

int quotient(int a, int b) {
    if (b != 0) return a / b;
    else {
        printf("Division by zero error!\n");
        return 0;
    }
}
```

### Remainder

```c
#include <stdio.h>

int remainder(int a, int b);

int main() {
    int a = 10, b = 5;
    printf("Remainder: %d\n", remainder(a, b));
    return 0;
}

int remainder(int a, int b) {
    if (b != 0) return a % b;
    else {
        printf("Division by zero error!\n");
        return 0;
    }
}
```

## 2. Function with Return Type and without Arguments

### Addition

```c
#include <stdio.h>

int add();

int main() {
    printf("Addition: %d\n", add());
    return 0;
}

int add() {
    int a = 10, b = 5;
    return a + b;
}
```

### Subtraction

```c
#include <stdio.h>

int subtract();

int main() {
    printf("Subtraction: %d\n", subtract());
    return 0;
}

int subtract() {
    int a = 10, b = 5;
    return a - b;
}
```

### Multiplication

```c
#include <stdio.h>

int multiply();

int main() {
    printf("Multiplication: %d\n", multiply());
    return 0;
}

int multiply() {
    int a = 10, b = 5;
    return a * b;
}
```

### Quotient

```c
#include <stdio.h>

int quotient();

int main() {
    printf("Quotient: %d\n", quotient());
    return 0;
}

int quotient() {
    int a = 10, b = 5;
    if (b != 0) return a / b;
    else {
        printf("Division by zero error!\n");
        return 0;
    }
}
```

### Remainder

```c
#include <stdio.h>

int remainder();

int main() {
    printf("Remainder: %d\n", remainder());
    return 0;
}

int remainder() {
    int a = 10, b = 5;
    if (b != 0) return a % b;
    else {
        printf("Division by zero error!\n");
        return 0;
    }
}
```

## 3. Function without Return Type and without Arguments

### Addition

```c
#include <stdio.h>

void add();

int main() {
    add();
    return 0;
}

void add() {
    int a = 10, b = 5;
    printf("Addition: %d\n", a + b);
}
```

### Subtraction

```c
#include <stdio.h>

void subtract();

int main() {
    subtract();
    return 0;
}

void subtract() {
    int a = 10, b = 5;
    printf("Subtraction: %d\n", a - b);
}
```

### Multiplication

```c
#include <stdio.h>

void multiply();

int main() {
    multiply();
    return 0;
}

void multiply() {
    int a = 10, b = 5;
    printf("Multiplication: %d\n", a * b);
}
```

### Quotient

```c
#include <stdio.h>

void quotient();

int main() {
    quotient();
    return 0;
}

void quotient() {
    int a = 10, b = 5;
    if (b != 0) printf("Quotient: %d\n", a / b);
    else printf("Division by zero error!\n");
}
```

### Remainder

```c
#include <stdio.h>

void remainder();

int main() {
    remainder();
    return 0;
}

void remainder() {
    int a = 10, b = 5;
    if (b != 0) printf("Remainder: %d\n", a % b);
    else printf("Division by zero error!\n");
}
```

## 4. Function without Return Type and with Arguments

### Addition

```c
#include <stdio.h>

void add(int a, int b);

int main() {
    int a = 10, b = 5;
    add(a, b);
    return 0;
}

void add(int a, int b) {
    printf("Addition: %d\n", a + b);
}
```

### Subtraction

```c
#include <stdio.h>

void subtract(int a, int b);

int main() {
    int a = 10, b = 5;
    subtract(a, b);
    return 0;
}

void subtract(int a, int b) {
    printf("Subtraction: %d\n", a - b);
}
```

### Multiplication

```c
#include <stdio.h>

void multiply(int a, int b);

int main() {
    int a = 10, b = 5;
    multiply(a, b);
    return 0;
}

void multiply(int a, int b) {
    printf("Multiplication: %d\n", a * b);
}
```

### Quotient

```c
#include <stdio.h>

void quotient(int a, int b);

int main() {
    int a = 10, b = 5;
    quotient(a, b);
    return 0;
}

void quotient(int a, int b) {
    if (b != 0) printf("Quotient: %d\n", a / b);
    else printf("Division by zero error!\n");
}
```

### Remainder

```c
#include <stdio.h>

void remainder(int a, int b);

int main() {
    int a = 10, b = 5;
    remainder(a, b);
    return 0;
}

void remainder(int a, int b) {
    if (b != 0) printf("Remainder: %d\n", a % b);
    else printf("Division by zero error!\n");
}
```

