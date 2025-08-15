# Elevate-Labs-Task-8
Online Quiz Application
Overview
This is a console-based Java application that implements a multiple-choice quiz. Users answer a series of questions, receive immediate feedback, and get a final score with performance feedback at the end.
Prerequisites

Java Development Kit (JDK): Version 8 or higher
IDE: VS Code or any Java-compatible IDE

Setup Instructions

Install JDK:

Download and install the JDK from https://www.oracle.com/java/technologies/javase-downloads.html
Ensure java and javac are available in your system's PATH


Project Setup in VS Code:

Create a new Java project
Place QuizApp.java in the src folder
Ensure VS Code is configured with the Java Extension Pack for proper compilation and running



Running the Application

Compile and run QuizApp.java in VS Code or via the command line:javac QuizApp.java
java QuizApp


The application will:
Display a welcome message
Present 5 multiple-choice questions with 4 options each
Accept user input (1-4) for each answer
Provide immediate feedback ("Correct!" or "Incorrect!" with the correct answer)
Show the final score, percentage, and performance feedback



Features

Question Management: Uses a Question inner class to store question text, options, and correct answers
Input Validation: Ensures user input is a number between 1 and 4, with error handling for invalid inputs
Scoring: Tracks correct answers and calculates the final score and percentage
Feedback: Provides motivational messages based on performance:
≥80%: "Excellent performance!"
≥60%: "Good job!"
<60%: "Keep practicing!"


Sample Questions: Includes 5 pre-defined questions on general knowledge and programming

Customization

Add Questions: Modify the initializeQuestions() method in QuizApp.java to add or change questions. Example:questions.add(new Question(
    "Your question here?",
    new String[]{"1. Option1", "2. Option2", "3. Option3", "4. Option4"},
    correctAnswerIndex // 1-4
));


Adjust Feedback: Change the percentage thresholds in the startQuiz() method to modify performance messages
Extend Functionality: Add features like question categories, timed quizzes, or saving scores by extending the code

Troubleshooting

Compilation Errors: Ensure JDK is installed and the Java path is correctly set
Input Issues: If the program skips inputs, ensure the console is active and you're entering numbers (1-4)
No Output: Verify that QuizApp.java is the main class being run

Notes

The application is console-based and requires no external dependencies
Questions are stored in memory and reset each time the program runs
The code uses an ArrayList for questions and Scanner for user input, with proper resource management
