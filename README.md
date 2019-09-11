# Worldfavor recruitment test

## Introduction
This repository is for Worldfavor's developer candidates only. 

It contains a basic `react` project to base the assignments upon. 

Candidates are required to go through the different assignments by providing their own implementation. 

A review meeting shall be held after receiving the candidate's code; questions may be asked regarding the code and the mindset displayed in the implementation. 

Plagiarism and collaboration are not only unethical but strongly discouraged. We ask that you clone the repo to your local disk and submit it back in a zip file to mitigate this.

This test should take no longer than 2h. 

If you feel you did not have the time to complete all the assignments and show all your capabilities, please submit your response for evaluation as the test is designed to asses various skill levels.

How to answer the different scenarios is open to the candidate unless stated in the question.

Be as true to yourself as you can, and good luck!

## Installation
In order to run this project you need to have a working `node` environment with `yarn` installed.

Clone this repository to your local machine and run:
```bash
yarn install
yarn start
```
A server should now be running on your machine with live update enabled, and you should be all setup for the assignments.

## Assignments
The different assignments are divided into multiple tasks; each task relies on the previous to work. 

Each task tackles a set of knowledge involved in our everyday development processes. 

To us, implementation design is as important as solving the assignment. 

The way you think will be first assessed through your code and further in a review meeting.

All assignments would ideally be completed without using external libraries, except for the one already available in `package.json`. 

No type definition nor linting are required from the candidate, but if you feel the need, we are open for this kind of initiatives.

Each task should be divided into its own folder, using the following naming convention: `task#`.

### Task 1

Using the provided design (in `design.png`), you are asked to reimplement the scene while supporting the following requirements:
- support an unknown amount of "network"
- have a responsive UI that display different number of "network card" depending on the screen resolution
- use `Material-UI` for small building blocks
- using the `Dialog` component from `Material-UI`, show a dialog containing the network name and description when clicking the network card

Mock data for the list of networks is provided in `mockData.js`. For this task, there is no need to use state management, only a direct access is enough.

We are not looking for a pixel perfect implementation, but we will be attentive to how true your implementation is to the design.

### Task 2

For this task, the candidate is asked to work on state management while supporting the following requirements:
- the header should include the first name of the user in place of `Welcome back, xxxx!`
- using Redux, implement reducer, actions and selectors to store and retrieve network objects
- store network data in the implemented state when the app is first loaded
- network objects have to come from the redux store whenever using them (no more direct access to `mockData.js`) 

### Task 3

For this task the candidate is asked to change the way the data is loaded, while supporting the following requirements: 
- load the data using an `axios` GET request (the requested url is not important)
- use the user token for the `Authorization` header of the request
- the response should be mocked using the data from `mockData.js`
