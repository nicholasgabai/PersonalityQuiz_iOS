# PersonalityQuiz_iOS
Personality Quiz IOS is a short interactive questionnaire to guess what animal type you are; based from App Development with Swift iBook.

## Part One—Project Planning

What features are required to produce a fun personality quiz? Since this is probably your first app of this type, keep the list short. At a minimum, the app should accomplish three main goals: 」

### Workflow

In this project, you'll update a single screen that can present all your questions, rather than presenting questions on separate screens.

### Controllers

Every UIViewController subclass you create is, in fact, a controller. A view controller uses the data model you've defined to control the view that's displayed on the screen. As your apps grow in complexity, you can create additional controllers to manage the model data, freeing up the view controller to focus only on view-related code. However, since this personality quiz has just three screens that contain very simple content, your view controllers can handle managing the data.

### Views

With a single view controller for all the questions and answers in your quiz, you'll want to display only the buttons, switches, slider, and/or labels that match the current question. The simplest and best way to do this is to group the controls within a view that corresponds to the question type. The appropriate view—for single-answer, multiple-answer, or ranged response—can then be shown or hidden.


## Part Two—Project Setup

### Create the Introduction Screen

The first view controller will invite the player to take your quiz. At a minimum, it needs to include a label that introduces the quiz and a button to begin. Beyond these simple requirements, the design of the screen is entirely up to you.

### Create the Question-and-Answer Screen

The second view controller will display each question, one at a time, along with input controls that allow the player to respond. The controls you use—buttons, switches, or sliders—need to make sense for the questions and answers in your quiz.

### Create the Results Screen

After the player has finished the quiz, the app will display the results, along with a short description. The player should have some way to dismiss the results and return to the introduction screen so that another player can take the quiz.


## Part Three—Create Questions and Answers

During the project planning phase, you considered three different question types: single-answer, multiple-answer, and ranged response. Now take some time to come up with your list of questions.

### Single-Answer Questions

### Multiple-Answer Questions

### Range Questions

### Question Label and Progress


## Part Four—Models and Outlets

So far in this lesson, you've designed the view controllers in the storyboard, and you've got three UIViewController subclasses ready to receive some code. Create structures that hold the question data and to update the user interface based on the values of each question and its answers. Once the data has been laid out, you can update the user interface based on which question is being displayed.

### Data Models

### Display Questions and Answers

### Display Questions with the Right Controls

### Update the Buttons and Label Text 

### Retrieve Answers with Actions


## Respond to Answered Questions


## Part Five—Calculate and Display Results 

The final steps include calculating the results, presenting them, and dismissing the results screen so that the quiz is ready for a new player. 」

### Pass Data to the Results View

The ResultsViewController also needs a property that can receive the data. This property will be used to calculate and present the final outcome of the quiz.

### Calculate Answer Frequency

Hw to calculate the personality. What was the most common personality type among the selected answers? In this example, if the player gave two answers that corresponded closely to dog and only one for each other animal, the best result would be dog. If two or more animals are tied for the most answers, either one would be a valid result.

### Determine the Most Frequent Answers 

Place each key/value pair into an array, sorting the value properties in descending order. 

### View the Results

Update the text of your labels to appropriate values inside calculatePersonalityResult.

### Restart the Quiz

In most personality quizzes, the player runs through all the questions once and only once. After the results have been displayed, there shouldn't be a way to go back and change previously answered questions to try and achieve a different outcome.

### Stretch Goals

Would you like to extend your personality quiz further?
