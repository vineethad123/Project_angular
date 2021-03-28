# Project_angular
Documentation:
Quiz application in one form or the other is becoming a general requirement for most of the applications these days. Be it Survey, mock test, preparation, self evaluation, gathering information, actual objective test or exam. This quiz application will help you to get through your need with minimal or no modification.
This presents you a simplified way to create your quiz application in Angular 11 in just few lines of code. The quiz application accepts the questions in json format. So, you can easily send the json from the server in the pre-defined format and the Angular quiz application will render the quiz at the client side. The quiz also has review and display result section. If you wish to declare the result immediately, you can simply call another json with the answers in it and simply evaluate and display the results immediately. Alternatively, if you wish to just submit the answers to the server, you can also do so at onSubmit method quiz.component.ts.
About Quiz:
The quiz application consists of mainly 3 components/views: Quiz View, Models, Services. For the sake of simplicity, I have kept the views in the same file.If you wish to scale this application, you can very well separate these views. Apart from this, quiz.component.ts has been used as a component class for all the views and styles.css has been used to apply CSS style to the application.
Quiz Running Logic:
The application has a small set of scripting part that has been handled by the controller: quiz.component.ts. First of all, the component loads the questions by using loadQuiz('data/aspnet.js') method called at ngOnInit event. The quiz questions should be provided in a pre-defined json format as mentioned in aspnet.json or other related json files present in data folder. Once the questions are loaded, user can answer the questions and the events are being captured by the same component. When user finally submits the quiz, you may submit the answers to the server in json format. Or load the questions with answers and evaluate the users answers to show the quiz result immediately. 
Quiz Configuration
The quiz configuration is an optional object that can be present in your <quiz>.json file. The config section allows you to customize your quiz the way you wish to do. The quiz application reads these configuration settings and applies these settings at the time of loading the quiz. The settings mainly consists of: shuffling the questions, showing/hiding pager, allowing back navigation, allowing auto move to next question. The details of this configuration is explained in "Quiz Features" section.
Services Used
For simplicity, I have used only one service in Angular2 component: quiz.service. It is used to retrieve quiz json file, populate the list of quizzes, and check the result.





