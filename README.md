# FILE-MANAGMENT-TOOL

COMPANY NAME: CODETECH IT SOLUTION

NAME: ABHAY KUMAR KINKAR

INTERN ID: CT04DF331

DOMAIN: C++

MENTOR: NEELA SANTOSH

#DISCRIPTION:

The provided C++ program is a simple yet effective File Management Tool designed to perform basic operations on text files. These operations include writing to a file, reading from a file, and appending data to a file. The program utilizes standard C++ libraries such as <iostream>, <fstream>, and <string> to handle input/output operations and manage files. This essay explains the structure, purpose, and flow of the program in detail, demonstrating how it serves as a practical example of file handling in C++.

At the beginning of the program, the #include directives import essential header files. The <iostream> library enables standard input and output functions such as cin and cout, while <fstream> provides facilities to read from and write to files. The <string> library is used to handle string inputs effectively using the std::string class. The using namespace std; line allows the programmer to use common names such as cout, cin, and string without prefixing them with std::.

The core logic of the program is divided into three separate functions: writeFile, readFile, and appendFile. Each function takes a single parameter, filename, which determines the file on which the operation will be performed.

The writeFile function allows the user to write new content to a file. When the file is opened using ofstream file(filename);, it clears any existing content and prepares the file to be overwritten. If the file fails to open, an error message is displayed. The program then prompts the user to enter a line of text. Before using getline(), the program calls cin.ignore() to remove any leftover newline characters in the input buffer from previous cin operations. The getline() function is used instead of cin so that multi-word or sentence input is captured correctly. Once the data is collected, it is written to the file, and the file is closed with file.close(). A success message is displayed to notify the user.

The readFile function is designed to read and display the contents of a file. The file is opened in input mode using ifstream file(filename);. If the file does not exist or cannot be opened for any reason, an error message is shown. The program reads the content line by line using a while loop and the getline() function. Each line read from the file is displayed using cout. After reading, the file is closed to free system resources.

The appendFile function allows the user to add new content to the end of an existing file. It opens the file in append mode using ofstream file(filename, ios::app);. This mode ensures that any new data is added to the end of the file without deleting its existing content. Like the writeFile function, it prompts the user for input, uses cin.ignore() to manage the input buffer, and then captures the input with getline(). The new data is written to the file, followed by a success message.

The main() function is the entry point of the program and handles user interaction. It begins by displaying a simple menu with three choices, each corresponding to a file operation. The user is prompted to enter a number between 1 and 3 and then provide the name of the file, including the .txt extension. Depending on the user's choice, the program uses a switch statement to call the appropriate function. If the input does not match any valid option, an error message is displayed.

In conclusion, this File Management Tool is a well-structured and beginner-friendly program that introduces the concept of file handling in C++. It effectively demonstrates how to open, write to, read from, and append to text files. The use of ifstream, ofstream, and appropriate file modes makes the program robust and functional. Through clear structure and user interaction, the program offers a practical way for learners to understand essential file operations in C++.
