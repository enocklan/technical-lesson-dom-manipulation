

Technical Lesson: DOM Manipulation
Overview

Scenario: Flatspace is a social media company that wants to work on features to personalize its users' account page. They want you to develop a function that will take an object of user information and display the details of the object onto a webpage. By manipulating the DOM along with the given object, we will be able to dynamically load the user information onto the webpage

Estimated Completion Time: 30-60 minutes

Instructions

Fork and Clone the Repository:

Go to the provided GitHub repository link.
Fork the repository to your GitHub account.
Clone the forked repository to your local machine.
Open the project in VSCode.
Run npm install to install all necessary dependencies.
Set up the starter variables:

Set up the starter variables of userInfo and displayUser
const userInfo = {
   username: "flatUser123",
   description: "Hi, welcome to my webpage! Just a new user of this website!",
   theme: "red"
}

function displayUser(userInfo){

}

displayUser(userInfo)
Select elements
Use querySelector to select Header
const userInfo = {
	username: "flatUser123",
	description: "Hi, welcome to my webpage! Just a new user of this website!",
	theme: "red"
}

function displayUser(userInfo){
	const header = document.querySelector("#main")
}

displayUser(userInfo)
Open the webpage for testing

To open the webpage using one of the following commands given your environment:
Local environment on Mac: Run open index.html in the terminal.
Local environment using WSL/Ubuntu: Run explorer.exe index.html in the terminal.
Edit text content

Use textContent to change the text of the title
const userInfo = {
	username: "flatUser123",
	description: "Hi, welcome to my webpage! Just a new user of this website!",
	theme: "red"
}

function displayUser(userInfo){
	const header = document.querySelector("#main")
	header.textContent = userInfo.username + "'s Personal Webpage"
}

displayUser(userInfo)
Change classname
Use className to change css class
const userInfo = {
	username: "flatUser123",
	description: "Hi, welcome to my webpage! Just a new user of this website!",
	theme: "red"
}

function displayUser(userInfo){
	const header = document.querySelector("#main")
	header.textContent = userInfo.username + "'s Personal Webpage"
	header.className = userInfo.theme
}

displayUser(userInfo)
Create and select elements
Create new element for description and select existing element of where it will go
const userInfo = {
	username: "flatUser123",
	description: "Hi, welcome to my webpage! Just a new user of this website!",
	theme: "red"
}

function displayUser(userInfo){
	const header = document.querySelector("#main")
	header.textContent = userInfo.username + "'s Personal Webpage"
	header.className = userInfo.theme

	const description = document.createElement("p")
	const body = document.querySelector("body")
}

displayUser(userInfo)
Add details
Add textContent and className to new element
const userInfo = {
	username: "flatUser123",
	description: "Hi, welcome to my webpage! Just a new user of this website!",
	theme: "red"
}

function displayUser(userInfo){
	const header = document.querySelector("#main")
	header.textContent = userInfo.username + "'s Personal Webpage"
	header.className = userInfo.theme

	const description = document.createElement("p")
	const body = document.querySelector("body")

	description.textContent = userInfo.description
	description.className = userInfo.theme
}

displayUser(userInfo)
Add new element to DOM
Append new element to existing element
const userInfo = {
	username: "flatUser123",
	description: "Hi, welcome to my webpage! Just a new user of this website!",
	theme: "red"
}

function displayUser(userInfo){
	const header = document.querySelector("#main")
	header.textContent = userInfo.username + "'s Personal Webpage"
	header.className = userInfo.theme

	const description = document.createElement("p")
	const body = document.querySelector("body")

description.textContent = userInfo.description
	description.className = userInfo.theme

	body.append(description)
}

displayUser(userInfo)
