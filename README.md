Software Architecture & Design
# MVC Calculator

Model-View-Controller (MVC) is one of the well-known architectural patterns typically used to develop user interfaces.

## About MVC
The Model-View-Controller (MVC) design pattern is a widely used architectural pattern in software development that separates an application into three interconnected components: Model, View, and Controller. This separation helps organize code, improve maintainability, and promote the concept of modularization.

Here's an overview of each component:

### Model
The Model represents the application's data and business logic. It is responsible for managing the data, processing business rules, and responding to requests for information about the application's state.

The Model notifies registered observers (usually Views) about changes in its state, allowing the Views to update accordingly.

In a well-designed MVC application, the Model should be independent of both the View and the Controller, promoting reusability and testability.

### View
The View is responsible for presenting the data to the user and receiving user input. It displays the information retrieved from the Model and sends user commands (e.g., button clicks, keyboard input) to the Controller for further processing.

Views are typically passive and don't contain much business logic. They rely on the Model to provide data and the Controller to handle user input.

Multiple views can be associated with a single model, allowing different representations of the same data.

### Controller
The Controller acts as an intermediary between the Model and the View. It receives user input from the View, processes it (possibly interacting with the Model), and updates the View accordingly.

The Controller is responsible for interpreting user actions and invoking the appropriate methods on the Model to update the application state.

In a well-designed MVC architecture, Controllers are decoupled from the Views, allowing for better reusability and testability.

## MVC Workflow

1. The user interacts with the View by providing input.
2. The View forwards the input to the Controller.
3. The Controller processes the input, possibly updating the Model.
4. The Model notifies the registered Views about any changes.
5. The Views retrieve the updated data from the Model and refresh their presentation.
6. The user sees the updated View and can interact with the application again.

The MVC design pattern helps to achieve separation of concerns, making it easier to modify or extend one component without affecting the others. It is commonly used in various frameworks and technologies, including web development (e.g., with frameworks like Ruby on Rails and Django) and desktop application development.

# MVC Exercise

📺 [Model-View-Controller (MVC) Exercise](https://youtu.be/YbPOTAeoPV4)

In this exercise, you are given a GUI-based Python implementation of a simple calculator (see the file `main.py`). The design follows the MVC pattern.

1. Download the file [`main.py`](./main.py) to your computer.
2. Study the code and understand the MVC structure.
3. Perform the following modifications to understand the structure further.
    1. Add a decimal point to the user interface so that the new calculator supports input and calculation of decimal point numbers.
    2. Support keyboard entry. In other words, the user can use the keyboard to input numbers and operations.
    3. Keyboard and mouse entry (clicking on buttons) must be able to run side by side.

I use [PyCharm Community Edition](https://www.jetbrains.com/pycharm/download/) when working on Python files.
