<h1>
  <span class="prefix"></span>
  <span class="headline">Create Expense App Lab</span>
  <span class="subhead">Exercise</span>
</h1>
## Overview

In this lab, you'll build an app that does CREATE, READ and DELETE (CRD) with `useState` and reuse of components.

## Prerequisites

- React Components
- State Management (including props)
- Lifting State

## Wireframe

You are to base the app on the wireframe outlined below.<br/>
<br />
![Expense App Wireframe](./assets/expense-app.png)


## Requirements

The app with be built with 7 components only:
- App
- Form
- Display
- Item
- Label
- Input
- Button

You can name the components any name you see fit.

## Functionality

The app will:
- store all expenses
- display all expenses to the user (READ).
- allow the user to add a new expense (CREATE).
- allow the user to delete an expense (DELETE)

## Sample Code for the Button component

```javascript
// Reusable Button component partial codes
const Button = (props) => {
  return (
    <button className={`btn ${props.className}`} 
      type="button" onClick={props.onClick}>

		{props.children}

	</button>
  )
}
```

## What is props.children

```javascript
// Partial Parent components to explain props.children
const Parent = (props) => {
  return (
    <Button>
      // Any jsx, Components, text, etc. in this area
      // between the open and close elements 
      // will be passed to the Button child
      // as props.children. 
      // props.children is create automatically.
    </Button>
  )
}
```

## Main Objective

In this lab, you will learn how to create and reuse components, manage state, prop data and lift state. In reuse, you will learn how to prop data into your child to change their look and functionality.

## Level Up

- Using today's date as default (codes below).

```javascript
const currentDate = new Date().toISOString().split("T")[0]
const [date, setDate] = useState(currentDate)
```

- Adding the UPDATE functionality.
