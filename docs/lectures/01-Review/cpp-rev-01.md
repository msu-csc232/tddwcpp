# Language Basics

Let's take a look a simple C++ program.

```c++
#include <iostream>
/**
 * Entry point of this application.
 */
int main()
{
    const double PI = 3.14159;
    double radius;

    std::cout << "Enter the radius of the sphere: ";
    std::cin >> radius;
    double volume = 4 * PI * radius * radius * radius / 3;
    std::cout << "The volume of a sphere of radius "
              << radius << " inches is " << volume
              << " cubic inches.\n";
    return EXIT_SUCCESS;
} // end program
```

We could compile this program as such:

```bash
$ g++ -std=c++11 foo.cpp
$ ./a.out
Enter the radius of the sphere: 3.4
The volume of a sphere of radius 3.4 inches is 164.636 cubic inches.
$
```
