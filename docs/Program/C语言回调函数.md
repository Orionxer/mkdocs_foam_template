---
title: C语言回调函数
date: 2024-10-15
type: feature
tags:
  - C
---

# C语言回调函数

## Demo
```C
#include <stdio.h>

// Define the callback function type
typedef void (*CallbackFunction)(void);

// A simple callback function
void my_callback() {
    printf("Callback function executed.\n");
}

// Function that accepts a callback and executes it
void execute_callback(CallbackFunction cb) {
    printf("Executing callback...\n");
    // Call the callback function
    cb();
    printf("Callback execution finished.\n");
}

int main() {
    // Pass the callback function to execute_callback
    execute_callback(my_callback);
    return 0;
}
```

