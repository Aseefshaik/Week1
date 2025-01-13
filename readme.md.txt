Dynamic Quiz App

Overview

The Dynamic Quiz App is a web-based quiz application that displays a series of questions, allows users to select answers, and tracks their score. The app also includes a timer for each question and the ability to restart the quiz at the end. The application saves the user's score in local storage to preserve it across sessions.

Features

Dynamic Questions: Displays questions and options dynamically from a predefined dataset.

Timer: A 30-second countdown timer for each question.

Score Tracking: Keeps track of the user's score.

Local Storage: Saves the score to local storage.

Restart Quiz: Option to restart the quiz after completion.

Files Included

HTML File: Contains the structure of the quiz app.

CSS: Embedded styles for the layout and design.

JavaScript: Script for dynamic functionality like loading questions, handling user input, and managing the timer.

How to Use

Open the HTML file in any modern web browser.

Read the question displayed and select an answer by clicking the corresponding button.

If the selected answer is correct, your score will increment.

If you do not answer within 30 seconds, the quiz will automatically move to the next question.

After all questions are answered, your score will be displayed.

Click the Restart Quiz button to retake the quiz.

Code Structure

HTML

#app: The main container of the application.

#quiz-container: Contains the quiz interface (questions, options, timer).

#results-container: Displays the final score and the restart button.

CSS

Provides styles for:

Centering the app on the page.

Styling the buttons and containers.

Hiding elements dynamically with the .hidden class.

JavaScript

Quiz Data:

Stored as an array of objects with question, options, and answer.

Main Functions:

loadQuestion: Loads the current question and options.

startTimer: Handles the 30-second countdown for each question.

checkAnswer: Checks the selected answer and updates the score.

nextQuestion: Moves to the next question or shows results.

showResults: Displays the user's final score.

restartQuiz: Resets the quiz to the initial state.

Event Listeners:

DOMContentLoaded: Loads the quiz on page load.

nextButton: Moves to the next question.

restartButton: Restarts the quiz.

How to Customize

Add Questions:

Update the quizData array in the JavaScript section with new question objects:

{
    question: "Your question here",
    options: ["Option 1", "Option 2", "Option 3", "Option 4"],
    answer: "Correct answer"
}

Change Timer Duration:

Modify the timeLeft variable in the JavaScript file.

Browser Compatibility

The app is compatible with modern browsers, including:

Google Chrome

Mozilla Firefox

Microsoft Edge

Safari

Future Enhancements

Add a progress bar to visually show the user's progress.

Include categories or difficulty levels.

Provide immediate feedback for correct/incorrect answers.

Enable question randomization.

License

This project is open-source and can be freely modified and distributed.