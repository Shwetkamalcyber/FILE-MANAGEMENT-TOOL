# FILE-MANAGEMENT-TOOL
COMPANY: CODTECH IT SOUTION 
NAME: SHWET KAMAL
INTERN ID: CT04DF161 
DOMAIN: C++
DURATION: 4 WEEKS
MENTOR: NEELA SONTASH

#DESCRIPTION:

The C++ File Management Tool is a command-line-based application designed to perform basic file operations such as writing to a file, reading from a file, and appending data to an existing file. Developed using fundamental C++ features, this tool provides an interactive and beginner-friendly way to understand file handling mechanisms in C++.

At the heart of the program lies the use of file stream classes provided by the <fstream> header in C++. Specifically, it uses three classes:
1. ofstream (output file stream) for writing to files,
2. ifstream (input file stream) for reading from files, and
3. fstream (file stream) for more advanced file handling, though not directly used in this program.

The program begins by displaying a menu that allows the user to choose an operation. The switch-case control structure is used to handle the selection, making the logic clean and easy to follow. Based on the user’s input, a specific function is called — writeFile(), readFile(), or appendFile() — each handling its respective task.

In the write operation, the program opens a file using ofstream in default mode, which overwrites any existing content in the file. The user is prompted to enter a line of text, captured using getline(cin, data) to allow spaces in input. The entered data is then written to the file using the insertion (<<) operator.

The read operation demonstrates the use of ifstream to read from a file. It employs a while loop to read the file line by line using getline(). This method ensures that the program can handle files with multiple lines and print them neatly to the console. It also shows how to detect if a file failed to open, using bv a simple if (!file) check.

In the append operation, the file is opened using ofstream with the ios::app flag. This tells the compiler to add new data at the end of the file without deleting the existing content. Again, getline() is used for input, and the entered text is added to the file with a newline character to maintain formatting.

The program also makes use of input handling techniques like cin.ignore() before using getline(). This is necessary because cin leaves a newline character in the input buffer after reading numeric input, which can cause getline() to skip the actual input. This reflects a deeper understanding of buffer handling in C++ input streams.

In addition to file operations, this tool reinforces several foundational C++ concepts such as function definition and calling, parameter passing by reference (using const string&), and basic error handling. Using const references ensures efficiency by avoiding unnecessary copying and promotes safety by preventing modifications to the original arguments.

Overall, this tool is an effective demonstration of how to manipulate files using C++. It highlights how streams work, how to structure a program using functions, and how to manage user input in a controlled way. 

#OUTPUT:

