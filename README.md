Download Link: https://assignmentchef.com/product/solved-problem-a-and-problem-b-computing-statistics-from-multiple-statistics
<br>
<span class="kksr-muted">Rate this product</span>

Problem A: Computing simple statistics on data residing in different files and recording the results in a file. (20 points)



In this problem, you will create a C++ program that reads in data from multiple different files that each store salary data in the same format; compute simple statistics on the data and write the Simple statistics your program computes out to a single output file (the output file your program creates is designed to be used in Problem B of this assignment).

Each file your program obtains input from will have the same format. Each file should contain a list of salaries from groups of workers who perform similar functions in a company (e.g., management, engineering, administrative assistance, and union-controlled manufacturing work).

For example, the file named a salaries . dat, which is one of the files that we gave you with this assignment, contains the following data:

45000.00

53000.00

58000.50

49000.00

55000.75

Your program should determine the following quantities for each file it reads:

The minimum salary value stored in the file

The maximum salary value stored in the file

The average value of all the salaries stored in the file

Once this is completed for an Input file, your program should output the name of the input file, and the results of the computations on the data stored in the input file (maximum salary, minimum salary, and average of all the salaries in the file), to the output file. Note, your program will write the results it computes for each input file into a single output file — that is, one output file will be used to store all the results.

Your program will then prompt the user to see if they would like to enter another input file for We have provided the following files for you to use as you carry out the analysis, design, implementation, and testing required to develop your solution to this problem:

asalaries.dat, esalaries .dat, msalaries.dat, and usalaries.dat

An example run illustrating how your program should behave is specified on the following page

— note, user input is in BOLD

Enter name of output file: results

Enter name of input file: asalaries

ERROR : can’t open input file: asalaries

Constraints:

The format and contents of the output file produced by your program (named result s in the example above) should be like the following:

45000.00

50000.75

130000.50

50000.00

58000.50

130000.00

52000.25

88400.30

190000.25 156000.53

80000.00 65600.00

Note, each line in the output file results is formatted at follows:

name of input file minimumsalary maximumsalary averagesalary

each of the values on a line is separated by at least one space, and there are no spaces in the file

More Constraints:

You must use a continuation loop as illustrated in the example input

You must use an indefinite loop to read in the values from each of the input files that your program processes

You must declare, define and use a non-pure function to obtain the name of the input file from the user and perform error checking (as illustrated in the example above). The non- pure function should return a void type, and accept two formal parameters, a string that will contain the filename m put by the user, and a file pointer object. Both parameters should be passed by reference the parameters will be set to values in the function (when your program obtains the name of the input file from the user and   successfully open the file) — and they will be used in the main function of your program.

Your program should close each input file after reading all the data in from the file

Your program should close the output file after the user decides to exit the program (e.g.,  is, the user responds n as in the example above)

Assumptions:

You can assume each input file will be have at least one salary, and all salaries will be  valid numeric values

You can assume No salary will be greater than dollars, or less than 1 dollar

You can assume salaries will have a decimal component.

Problem B: Computing Statistics from Multiple Statistics (20 points)

In problem A of this Homework assignment. the objective is to write a program to compute statistics on data (salaries) stored m in the same format in different files, and store the statistics

computed from the data stored in each Input file m a single output file containing all the results.

In this problem, you will write a program to compute statistics on the data stored in the format specified in the results file shown in problem A above.

Specifically, your program should read the data in from a file with 1 or more lines of data in the following format:

string number I number2 number 3

s is the name of the file from which the values number1, number2, and numbed

were computed

number 1 is the minimum average salary extracted from the data in the file

number 2 is the maximum average salary extracted from the data in the file

number 3 is the average salary computed from the list of salaries in the file

For example, the file named results shown below contains data in the format specified above, and was produced from the example files asalaries . dat, esalaries . dat,

msalaries . dat,

asalaries . dat

esalaries . dat

msalaries . dat

usalaries . dat

and usalaries . dat provided for Problem A in this assignment

45000.00

50000.00

130000.50

50000.00

58000.50 52000.25

130000.00 88400.30

190000.25 156000.53

80000.00 65600.00

Your program should prompt the user for the name of a file containing data that adheres to the format specified above, open the file and then compute.

The Minimum Salary and the filename that held the value

The Maximum Salary and the filename that held the value

The Minimum Average Salary and the filename that held the value

The Maximum Average Salary and the filename that held the value

The Average of all salaries.

Once the values above are obtained by your program, your program should output them to the console.

An example run Illustrating how your program should behave is specified below — note, user input is m BOLD:

Enter name of input file: results

Minimum Salary found: 45000 .00 in File: asalaries . dat

Maximum Salary found: I goooo .25 in File: msalaries. dat

Minimum Average Salary found: 52000.25 in File: asalaries . dat

Maximum Average Salary found: 156000 .53 in File: msalaries . dat

Average of all salaries: 90500.27

Continue? (Enter ‘Y’ or ‘y’): n

Constraints:

The format and contents output to the console by your program should be like the output shown above

You must use a continuation loop as illustrated in the example input

You must use an indefinite loop to read in the values from each of the input files that your program processes

You must declare, define and use a non-pure function to obtain the name of the input file from the user and perform error checking (as illustrated in the example above). The non- pure function should return a void type, and accept two formal parameters, a string that will contain the filename m put by the user, and a file pointer object. Both parameters should be passed by reference. The parameters will be set to values in the function (when your program obtains the name of the input file from the user and successfully open the file) — and they will be used in the main function of your program.

Your program should close each input file after reading all the data in from the file

Assumptions:

You can assume each input file will be have at least one salary: and all salaries will be valid numeric values.

You can assume No salary will be greater than dollars, or less than 1 dollar