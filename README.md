### ***Title*** : LAB10
### ***Aim*** : 
(1) Reading from an xcel(.csv) file Name and Age using r(read) mode and storing as structure using malloc dynamic memory allocation

(2) Writing to a file Name and Age using a(append) mode

### ***Algorithm*** :

Reading from a CSV File and Storing as a Structure

***Algorithm for part1***:

Open the CSV file for reading.

Check if the file was opened successfully. If not, display an error message and exit.

Create a structure (in this case, Person) to store the data from each line of the CSV file. The structure contains two members: a character pointer for the name and an integer for the age.

Create a vector or another suitable data structure to hold instances of the Person structure.

Read each line from the CSV file using std::getline.

Tokenize the line by splitting it at each comma (,). For this, you can use strtok.

Extract the name and age from the tokens and store them in a new instance of the Person structure.

Add the Person structure to your data structure (e.g., a vector) if the tokenization is successful.

Print the data from the data structure (e.g., the vector).

Free the dynamically allocated memory to prevent memory leaks.

Writing to a File in Append Mode

***Algorithm for part2***:

Open the file in append mode using ofstream with the ios::app flag.

Check if the file was opened successfully. If not, display an error message and exit.

Create a structure (in this case, Person) to store the data to be written to the file. The structure contains a string for the name and an integer for the age.

Input the name and age from the user.

Write the name and age to the end of the file using the << operator.

Close the file.


### ***Explanation*** :

***Explanation for part1***:

This program opens a CSV file, reads each line, splits it into name and age using comma as the delimiter, and stores this data in a dynamic data structure. It takes care of memory allocation and memory deallocation to avoid memory leaks. The extracted data is printed to the console.

***Explanation for part2***:

This program opens a file in append mode, allowing new data to be added to the end of the file without overwriting the existing content. It then prompts the user to input a name and an age. After obtaining this data, it writes the information as a new line in the file. If the file does not exist, it will be created. This program is suitable for adding records or appending data to an existing CSV file.

Both programs work with a Person structure for storing name and age, and they take care of file handling, memory allocation (in the reading program), and data input/output.

### ***Output Screenshot*** :
Code:

https://github.com/anikethmehta/LAB10/blob/main/code_part1_1.png

https://github.com/anikethmehta/LAB10/blob/main/code_part1_2.png

https://github.com/anikethmehta/LAB10/blob/main/code_part1_3.png

https://github.com/anikethmehta/LAB10/blob/main/code_part1_4.png

https://github.com/anikethmehta/LAB10/blob/main/code_part2_1.png

https://github.com/anikethmehta/LAB10/blob/main/code_part2_2.png

https://github.com/anikethmehta/LAB10/blob/main/code_part2_3.png

https://github.com/anikethmehta/LAB10/blob/main/code_part2_4.png

Output:

https://github.com/anikethmehta/LAB10/blob/main/output_part1.png

https://github.com/anikethmehta/LAB10/blob/main/output_part2.png

https://github.com/anikethmehta/LAB10/blob/main/excel_output_part2.png
