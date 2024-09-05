A1

Question #1: Display a message
Write a complete C++ program that displays the following output exactly as in the sample output. 
You are to use a single cout statement to output the message. 
There is no need to declare any variables for this question

Question #2: Number Generator Program

In C++, we can use rand() function (More details) to generate random numbers. In the question, 
we will generate a 3-digit random number between 100 – 999 and complete number calculation following the requirements:

1. Display a welcome message.
2. Display the randomly generated even/odd number.
3. Calculate the sum of the 3 digits in the number. For example, the addition of 3 digits in the number 345 is 3 + 4 + 5 = 12.
4. Calculate the subtraction of the 3 digits in the number. For example, the subtraction of the 3 digits in the number 345 is 3 - 4 - 5 = -6
5. Calculate the multiplication of the 3 digits in the number. For example, the multiplication of the 3 digits in the number 345 is 3 * 4 * 5 = 60
6. Calculate the reminder of the number divided by the sum of its 3 digits. For example, If the number is 345, then the reminder is 345%(3 + 4 + 5) = 9
7. Display a farewell message to indicate the program has terminated normally.

Use at least one constant variable to store value in the program.

Following are 2 sample screen shots to illustrate the expected behavior of your program.

Note: Your program must display the same information and formatted the same.

Question #3: New Word Program
Write a program that prompts the user for four words.

Your program should behave as follow:
1. Display a welcome message.
2. Ask the user to prompt 3 words with at least 1 letter.
3. Ask the user to prompt 3 numbers, that should be less than the length of each word to indicate length of
   substring in each word. For example, if the word is Ann, then the entered number should be less than 3 (the length of Ann).
4. Create a new word, which merges the substring of 3 words. If the entered number is even, the substring
   starts from the first letter; if is it odd, the substring starts from the second letter.
5. Display the resulting new word.
6. Display a farewell message, so that the user knows that the program has terminated normally.
Restriction: This questions requires the use of the functions: length(), substr().
Assumption: Assume a perfect user who will always enter the correct input values.

A2

Question #1: Covid Vaccine Program

In this question, you are asked to write a program to understand natural language. The user will enter the input following the format:
FirstName_LastName@Number1#Number2

For example:
Robin_Moring@1#2

Assume a perfect user will follow the exactly above formats for the inputs. 
Your program should be able to analyze the key words (Name, Number1 and Number2) from the inputs and display the outputs in the following format. 
You must use if-else statement to display the correct place.

LastName, FirstName has completed Number2 dose(s) of Covid 19 vaccine at Place*.

If the Number2 is less than 3, your program should also display the following message:

Please complete the remaining N** dose(s) soon. Take care!

If the Number1 is not listed in the table or Not Available, your program should ask user for a new input.

** N = 3 – Number2
* Here is a list of Place that your program should display according to the input Number1.

Hints: You may use string functions: at(), length(), substr(), stoi(), find() to solve this question.
Your program should be able to ask user for new input of user’s information for estimation until get the input Yes from the user. Following are sample screen shot to
illustrate the expected behavior of your program. User input at the keyboard is marked with a red circle.

Question #2: Covid Vaccine Appointment Program

In this question, you will write a program to help the resident book Covid vaccine program. Here are the detail requirements that your program should follow:

If you completed 3 doses, you do not need to book any appointments.

If you completed less than 3 doses, you need to book the appointment based the user’s entered age.

The program prompts the user to the choice based on the above table and validates the information according to the following rules:

− If the user’s entered age is not in the above range, ask the user enter again until receiving a valid input.
− Your program should check user’s entered number of locations and schedules. If it is not in the list, ask the user enter again.
− Display the complete appointment info if it is booked successfully.
− Display welcome/closing messages.

If the user give an invalid input of choice, your program should output message and ask user for a new one until a valid input is given.

A3

Programming Exercise #1 – File I/O

The file A3Q1_student.txt (included in downloaded handout) contain a list of studentID, courseName and GPA at Concordia University.

Write a program that allows the user to input a studentID. Your program should read and search for matching ID number in the list. 
If a match is found it should calculate the average GPA and write the studentID and average GPA in the file (output.txt). 
Your program should also indicate if there is no match (see Figure3).

Your program also must follow the requirements:
• Your program cannot open the data file. Figure1 illustrates the expected behavior.
• Your program calculate the average GPA received from the same studentID with all the taken courses in the given file and write into the file output.txt.
• Your program should write the complete studentID, list of courses and average GPA information into output.txt.
• Please note your program must use the same file name (A3Q1_student.txt and output.txt) to read and write the files. Figure 2 & 3 illustrate the expected behaviors.

Programming Exercise #2 – Covid Vaccine Appointment Program
In this question, you will continue working on Covid vaccine appointment program to help the residents book Covid vaccine appointments. 
Here are the detail requirements that your program should follow:

If you completed 3 doses, you do not need to book any appointments.
If you completed less than 3 doses, you need to book the appointment based the user’s entered age.

Here is a list of age, possible appointment starting dates, locations, and schedules. 
You must use a switch statement to find and display the correct location and schedule.

The program prompts the user to the choice based on the above table and validated the information according to the following rules:

• If the user’s entered age is not in the abo range, ask the user to enter again until receiving a valid input.
• Your program should check the user’s entered number of locations and schedules. If it is not in the list, ask the user to enter again.
• Display the complete appointment info if it is booked successfully.
• Display welcome/closing messages.

If the user gives an invalid input of choice, your program should output a message and ask the user for a new one until a valid input is given.

Here is a list of the functions you are required to create (as per specification) and use to solve this problem. You can create and use other functions as well if you wish.

1. Function Name: displayHeader()
• Parameters: None
• Return: None
• Purpose: This function will display the welcome banner.

2. Function Name: displaySchedule()
• Parameters: None
• Return: None
• Purpose: This function displays the vaccine schedule info to the user.

3. Function Name: getVaccineDose()
• Parameters: None
• Return: the valid choice from user
• Purpose: This function prompts them for a valid vaccine dose (0-3). It will continue prompting until a valid choice has been entered.

4. Function Name: processMenuChoice()
• Parameters: The variable that holds the choice of age, location and schedule entered by the user, passing by value; The variable that holds the starting date, location and schedule values, passing by reference.
• Return: none
• Purpose: This function will call the appropriate function based on the choice that is passed.

5. Function Name: getAgeInfo()
• Parameters: The variable that holds the choice of age.
• Return: the starting date.
• Purpose: This function asks the user’s valid input of age. Your program should use if-else statement to find the correct location.

6. Function Name: getLocationInfo()
• Parameters: The variable that holds the choice of location.
• Return: The schedule time
• Purpose: This function asks the user’s valid input of location. Your program should use if-else statement to find the correct location.

7. Function Name: getScheduleInfo()
• Parameters: The variable that holds the choice of schedule.
• Return: the schedule time
• Purpose: This function asks the user’s valid input of schedule. Your program should use only if statement to find the correct schedule.

8. Function Name: displayResult()
• Parameters: The variables that hold the age, starting date, location and schedule info in main, passing by value.
• Return: none.
• Purpose: This function displays the booked vaccine information.

A4 
Question #1: Writing a ‘structure’ declaration
a) Declare a struct type name Meeting which will describe an item. The following information should be included:

Name (string of characters)
Date (string of characters)
Capacity (integer number)
Mode (integer number) // 1 for online, otherwise it is in person
isOnline (Boolean) // only if the value of Mode is online.

b) Declare meeting1 to be a variable of type Meeting.

c) Write a function to read the first 4 values (Name, Date, Capacity and Mode) into the member variables of type Meeting.
(The struct variable should be passed as an argument) The order in which the data is read is the same as that of the items in the struct.

d) Your program should be able to ask for the user to enter another meeting’s information until the received answer is no. 
Display all the values on the console. Please note when displaying the capacity of the student(s), 
the single (capacity =1) or plural (capacity >1) form depends on the entered capacity. (see Figure below for the details)

Question #2: Implementing a class
a) A Meeting object represents the name, date, capacity and mode. Write a declaration for the class Meeting including its data members and 
function members based on the following UML and save it in a file called Meeting.h.

b) Implement the member functions based on the following descriptions, and save them in a file called Meeting.cpp.
• Meeting (): default constructor, which will set three attributes name, date, mode and capacity to “COMP218”, 2022-02-12, 0 and 100
• Meeting (string name): a name constructor which sets the attribute name to the passed value and the other three attributes date, mode and capacity will be the default one, which are 2022-02-22, 1 and 1.
• Meeting (string name, string date, int mode, int capacity): a third constructor which sets all the attributes to the passed values.
• getName(): returns the name of the meeting.
• getDate(): returns the date of the meeting.
• getMode(): returns the mode of the meeting.
• getCapacity(): returns the capacity of the meeting.
• setName(string n): sets the name attribute to n.
• setDate(string d): sets the date attribute to d.
• setMode(int m): sets the mode attribute to m.
• setCapacity(int c): sets the capacity attribute to c.
• changeOnline(int number): ask the user to change the in person meeting online. Number to indicate which meeting to be changed.
• isOnline(int m): returns true if the mode is online, otherwise false.
• equals(Meeting m): returns true if the name, date and mode of the calling objects are the same as the name, date and mode of the passed object m, otherwise false.
• postpone(string newDate): chage date attribute to newDate accordingly.
• printInfo(): display on the console the item name, date, price and quantity. (see the example below)

c) write a program name A4Q2.cpp that uses the class Meeting as follows:
• Create an object meeting1 using the default constructor.
• Create an object meeting2 using the second constructor. Prompt the user for the name. assume the user enters valid input.
• Create and object meeting3 using the third constructor. Prompt the user for the name, date, mode and capacity. Assume the user enters valid inputs.
• Display the meeting of three objects following the format shown in the example shown below.
• Check the 3 objects (meeting1, meeting2, meeting3) whether they are online. If the meeting is in-person, ask the user whether they want to change it online. Display all the meeting info.
• Create an integer array to save the capacity of 3 objects (meeting1, meeting2, meeting3). Calculate and display the total capacity of 3 meeting by using the array.
• Change the capacity of the second object meeting2 which equals to the sum of meeting1 and meeting 3. Update and display the total capacity of 3 meetings by using the array.
• Ask the user to postpone the meeting1.
• Compare the 3 objects (meeting1, meeting2, meeting3) and indicate whether they are equal. See format of message in the sample output at the end of this question.
• Print all the meeting info.
• End with closing message.

Note: Be sure to save the class declaration in a header file Meeting.h, the class implementation in a Meeting.cpp file. Don’t forget to include these files in the project.

