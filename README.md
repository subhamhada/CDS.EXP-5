# Experiment-5
## Aim -
To study and implement C++ decision making statements
## Theory -
Decision-making statements control the flow of a program based on conditions. Key types include:
### 1. *If-Else Statement*:
Executes one block if the condition is true, another if false.
### 2.*Nested if-else statements*:
these are used when you need to check multiple conditions in a hierarchical manner. An if or else block can contain another if-else statement inside it. This is useful for more complex decision-making processes.
### 3. *calculator statement*:
it is used for doing mathematical calculations among some given values.
### 4. *Switch Case Statement*: 
Used in some languages to handle multiple conditions, mimicked in Python using dictionaries.

## code -
### 1. *If-Else*
```
//subham
//23070123132
//entc b2
#include <iostream>
using namespace std;
int main() 
{
    double n1, n2, n3;
    cout << "Enter three numbers: ";
    cin >> n1 >> n2 >> n3;
    if(n1 >= n2 && n1 >= n3)
        cout << "Largest number: " << n1;
    else if(n2 >= n1 && n2 >= n3)
        cout << "Largest number: " << n2;
    else 
        cout << "Largest number: " << n3;
        return 0;
}
```

### 2. *Nested if else*
```
//subham
//23070123132
//entc B2
//experiment 5
#include <iostream>
using namespace std;
int main() 
{
    double n1, n2, n3;
    cout << "Enter three numbers: ";
    cin >> n1 >> n2 >> n3;
    if (n1 >= n2) 
    {
        if (n1 >= n3)
            cout << "Largest number: " << n1;
        else
            cout << "Largest number: " << n3;
    }
    else {
        if (n2 >= n3)
            cout << "Largest number: " << n2;
        else
            cout << "Largest number: " << n3;
    }
    return 0;
}
```

### 3. *Calculator*
```
//subham
//23070123132
//entc B2
//experiment 5
#include<iostream>
using namespace std;

int main() {
    char oper;
    float num1, num2;

    cout << "Enter an operator (+, -, *, /): ";
    cin >> oper;
    cout << "Enter two numbers: " << endl;
    cin >> num1 >> num2;

    switch (oper) {
        case '+':
            cout << num1 << " + " << num2 << " = " << num1 + num2 << endl;
            break;
        case '-':
            cout << num1 << " - " << num2 << " = " << num1 - num2 << endl;
            break;
        case '*':
            cout << num1 << " * " << num2 << " = " << num1 * num2 << endl;
            break;
        case '/':
            if (num2 != 0)
                cout << num1 << " / " << num2 << " = " << num1 / num2 << endl;
            else
                cout << "Error! Division by zero." << endl;
            break;
        default:
            cout << "Error! The operator is not correct" << endl;
            break;
    }

    return 0;
}
```

### 4. *Switch case*
```
//subham
//23070123132
//entc B2
//experiment 5
#include<iostream>
using namespace std;

int main()
{
    int choice;
    cout << "1. Monday" << endl
         << "2. Tuesday" << endl
         << "3. Wednesday" << endl
         << "4. Thursday" << endl
         << "5. Friday" << endl
         << "6. Saturday" << endl
         << "7. Sunday" << endl;
    cout << "Enter your choice: ";
    cin >> choice;
    
    switch(choice) {
        case 1:
            cout << "Monday" << endl;
            break;
        case 2:
            cout << "Tuesday" << endl;
            break;
        case 3:
            cout << "Wednesday" << endl;
            break;
        case 4:
            cout << "Thursday" << endl;
            break;
        case 5:
            cout << "Friday" << endl;
            break;
        case 6:
            cout << "Saturday" << endl;
            break;
        case 7:
            cout << "Sunday" << endl;
            break;
        default:
            cout << "Wrong Input" << endl;
            break;
    }
    
    return 0;
}
```

## Explanation:-
*if else*: statement for executing a block if it is true otherwise for false.

*nested if else*: are used when you need to check multiple conditions in a hierarchical manner.

*calculator statement*:is used for doing mathematical calculations among some given values.

*Switch Case Statement*: Used in some languages to handle multiple conditions, mimicked in Python using dictionaries.

## Output:-
### 1. *If else*
![Screenshot 2024-08-01 233510](https://github.com/user-attachments/assets/759a1bbf-c527-4f1c-8eb8-37201c7cbff3)

### 2. *Nested if else*
![Screenshot 2024-08-01 233730](https://github.com/user-attachments/assets/6b2360ff-c495-4c8b-b111-ec9af46d8c40)

### 3. *Switch*
![Screenshot 2024-08-01 233814](https://github.com/user-attachments/assets/69ce62e3-b41e-48bf-a0e9-920d3b0a31cf)

### 4. *Calculator*
![Screenshot 2024-08-01 233854](https://github.com/user-attachments/assets/a41ab5bd-23df-4bd5-987c-d8a00ffae76a)

## Conclusion:-
Decision-making statements in programming control the flow of execution based on conditions. The if-else statement executes different code blocks depending on whether a condition is true or false, while the nested if else statement allows for multiple conditions to be checked in sequence. The switch statement provides a way to select one of many code blocks to execute based on the value of an expression, ideal for handling discrete values. calculator helps in doing mathematical operations.
