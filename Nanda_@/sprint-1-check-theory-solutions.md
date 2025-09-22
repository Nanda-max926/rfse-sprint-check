### 1. Early computers were mechanical devices that used physical gears. The shift to electronics began with machines like the ENIAC, which used vacuum tubes to perform calculations much faster. The invention of the transistor then made computers smaller, more reliable, and more energy-efficient, leading to the personal computers we use today.

### 2. A Command-Line Interface (CLI) can be much faster for repetitive tasks. For example, a single command like `cd` can instantly navigate to a nested folder, whereas a Graphical User Interface (GUI) would require multiple clicks. Additionally, the CLI allows for powerful automation through scripting, which is not easily done in a GUI.

### 3. * Open your terminal and type `vim hello.txt`. 

   * Press `i` to enter Insert Mode.  

   * Type your text, such as `Hello, world!`.  

   * Press `Esc` to exit Insert Mode. 

   * Type `:wq` and press Enter to save and quit.

### 4. * `ls`: Lists the files and directories in the current location. 

   * `cd`: Changes the current directory.  

   * `pwd`: Prints the current working directory. 

   * `mkdir`: Creates a new directory. 

   * `touch`: Creates a new empty file.


### 5. A version control system (VCS) tracks changes to code over time, allowing you to easily revert to previous versions and preventing data loss. For a solo coder, if you're building a website and a new feature breaks the site, you can use a VCS to quickly and safely revert to the last working version of the code.

### 6. `git commit` saves a snapshot of your changes to your local repository on your computer. `git push` uploads those committed changes from your local repository to a remote repository, such as on GitHub.

### 7. * Go to the GitHub website and sign in. 

   * Click the "+" button and select "New repository". 

   * Give the repository a name and a description, then click "Create repository".

   * On the next page, click "uploading an existing file". 

   * Drag and drop your file into the box and add a commit message.

   * Click "Commit changes".

### 8. Python and JavaScript are high-level languages that are easier for beginners because they use syntax that is more similar to human language. They also handle complex, low-level details like memory management automatically, allowing beginners to focus on learning the logic of programming.

### 9. A compiler translates an entire program into machine code at once before it runs, like with C++. An interpreter translates and executes the code line by line as the program is running, like with Python.

### 10. A Just-In-Time (JIT) compiler compiles code during execution, turning it into machine code right before it's needed. Unlike a traditional compiler that compiles everything beforehand, a JIT compiler offers a balance of the flexibility of an interpreter and the speed of a compiler by only compiling and optimizing the parts of the code that are used most often.

### 11. A transpiler is a tool that converts source code from one programming language into source code of another language. For example, Babel transpiles modern JavaScript code (like using `const` and arrow functions) into older JavaScript that is compatible with more web browsers.

### 12. * Efficient: The software uses resources like memory and CPU effectively. 

   * User-friendly: It is intuitive and easy for people to use. 

   * Reliable: It works as expected without crashing or errors.
   

### 13. You can use benchmarking. This involves running both programs on the same tasks and hardware while measuring the time it takes to complete them (for speed) and monitoring the amount of memory they use (for memory usage) with specialized tools.

### 14.  
           function is_prime(number):  
               if number <= 1:  
                  return false  
                    for i from 2 to sqrt(number):  
               if number % i == 0:  
                   return false  
                  return true

### 15. When the CPU needs data, it requests it from a specific memory address in the RAM.

### 16. In strictly typed languages like Java, you must declare a variable's type, and it cannot change. For example, `int myNumber = 10;`. In loosely typed languages like Python, you don't declare the type, and it can change. For example, `my_number = 10` can later become `my_number = "hello"`.


### 17. Integer age = 30  

    Float price = 19.99  

    char initial = 'A'  

    string name = "John Doe" 

    boolean is_complete = false


### 18. * A kernel is the central part of the operating system that manages hardware. 

    * A process is an instance of a running program.  

    * A thread is a single sequence of instructions within a process. 

   *  A core is a physical processor on a CPU.


### 19. * New: The thread has been created but not yet started.  

    * Runnable: The thread is ready to run and is waiting for the CPU.  

    * Running: The thread is currently executing its code.  

    * Blocked: The thread is paused, waiting for a resource to become available.


### 20. Concurrency is about a single person juggling multiple tasks by switching between them quickly, like one chef preparing different parts of a meal at the same time. Parallelism is about doing multiple tasks at the exact same time using multiple resources, like a team of chefs each cooking a separate dish simultaneously.

### 21. A byte (8 bits) became the standard unit of data storage. The original ASCII standard only needed 7 bits to represent 128 characters. Storing one character in a single byte was a practical and efficient way to use memory, with the extra bit later used for extended characters.

### 22. ASCII is a character encoding standard that uses a unique number to represent each character. The uppercase letter "A" is encoded with the decimal value 65, which is 01000001 in binary.

### 23. While ASCII only used 7 bits, hardware was more efficient at processing data in 8-bit chunks. This standardization around the 8-bit byte simplified computer architecture and allowed for an extended set of characters to be represented using the 8th bit.

### 24. Functions are useful because they allow you to organize and reuse code. Instead of rewriting the same logic, you can define it once in a function and call it whenever needed. For example, a function `add(a, b)` can be used repeatedly to add any two numbers without having to rewrite the `a + b` logic each time.

### 25. function sum(a, b):  
     return a + b  

     // Main program  
     number1 = 5  
     number2 = 10  
     result = sum(number1, number2)  
     print("The sum is: " + result)

### 26. Formal parameters are the placeholders in a function's definition, like `name` in `function greet(name)`. Actual parameters are the real values passed into the function when it's called, like `"Alice"` in `greet("Alice")`.

### 27. * Register (fastest) 

   * Cache  

   * RAM 

   * Storage (slowest)


### 28. Stack memory is fixed because its size is determined at compile time for things like local variables and function calls. Heap memory is dynamic because its size can change during runtime to handle data whose size isn't known beforehand, like an array created with a size entered by the user.

### 29. A pointer is a variable that stores a memory address.

### 30. A pointer is a variable that stores a memory address. For example, if you have a variable 
       `x = 5`, a pointer `p` can store the memory address where the value `5` is located.

### 31.  
           function assign_grade(score):  
             if score >= 90:  
                return "A"  
            else if score >= 80:  
                return "B"  
            else if score >= 70:  
               return "C"  
            else:  
               return "D"

### 32. Use a switch statement when you need to check a single variable against a series of specific, fixed values. It makes the code cleaner and more readable than a long if-else chain. 

       Example:  
      print("1. New Game")  
      print("2. Load Game")  
      print("3. Quit")  
      input choice = get_user_input()  

              switch choice:  
               case 1:  
                 start_new_game()  
                  break  
                case 2:  
                 load_game()  
                  break  
               case 3:  
                 quit_game()  
                  break  
               default:  
                 print("Invalid choice")

### 33.  
             function check_eligibility(age, has_id):  
               if age >= 18 and has_id == true:  
                  print("You are eligible.")  
               else:  
                  print("You are not eligible.")

### 34.  
        function compare_numbers(num1, num2):  
               if num1 > num2:  
                  else if num1 < num2:  
                      print(num1 + " is less than " + num2)  
                        else:  
                     print(num1 + " is equal to " + num2)
 
### 35.  
            for row from 1 to 3:  
             for column from 1 to 3:  
             print("* ")  
             print("") // New line after each row

### 36.  
          integer sum = 0  
         integer i = 1  
         while i <= 10:  
          sum = sum + i  
          i = i + 1  
           print("The sum is: " + sum)

### 37.  
         for i from 1 to 10:  
           if i % 2 == 0:  
             continue // Skips to the next iteration  
             print(i) // Only odd numbers will be printed
      

### 38. A simple variable stores a single piece of data, like `age = 30`. An array is a structured collection that stores multiple items of the same type under a single name, like `ages = [25, 30, 35]`. The key difference is that a variable holds one value, while an array can hold many.

### 39. Imagine an array as a list of items. Most of the time, adding an item is very fast. However, when the array is full, the computer has to create a completely new, larger array and copy all the old items to the new one. This is a very slow operation. Amortized analysis is the way of averaging the cost of that one slow "copy" operation over all the many fast "add" operations that came before it. This shows that the average cost per "add" is actually very low.

### 40. O(n) means that the runtime of an algorithm grows linearly with the size of the input. If the input list doubles in size, the time it takes to run also roughly doubles. For example, a single loop that iterates over every item in a list to find a specific value has a time complexity of O(n) because it has to perform an operation for each of the n items.
