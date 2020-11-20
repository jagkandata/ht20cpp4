# Uppgift 1

Skriv klart följande program:

```c++
#include <iostream>

void add(double &num, double add);
void subtract(double &num, double sub);
void multiply(double &num, double multiplier);
void divide(double &num, double divider);

int main(){
  int num = 10;
  
  add(num, 10);
  std::cout << "num har nu värdet: " << num << std::endl; // ska skriva ut 20
  subtract(num, 10);
  std::cout << "num har nu värdet: " << num << std::endl; // ska skriva ut 10
  multiply(num, 2);
  std::cout << "num har nu värdet: " << num << std::endl; // ska skriva ut 20
  divide(num, 2);
  std::cout << "num har nu värdet: " << num << std::endl; // ska skriva ut 10
  
  return 0;
}
```

# Uppgift 2

Skriv klart följande program:

```c++
#include <iostream>


bool createPerson(Person &person);

int main() {
    Person person;
    char answer;
    
    do{
        createPerson(person);

        std::cout << person.firstName << " " << person.lastName << " is " << person.age << " years old." << std::endl << std::endl;

        std::cout << "Create another person? (Y/N)";
        std::cin >> answer;
        
        
    }while(answer == 'Y' || answer == 'y');

    return 0;
}

```
