# React Assessments

Try your best to answer each question on your own before looking up the answer online. Once you're done writing your first answer, you can google the question and write the best answer you find.

#### 1. Here is a list of pros and cons to using the React library to build your application -- but some of them are false. Remove the false statements from the list:

<!--- FALSE: React was created to be simple, so that even people with minimal code experience could use it and create Single Page Applications (SPAs)-->

- React is a modern, efficient answer to complex UI applications

<!--- FALSE: React is a full stack framework for modern web applications-->

- React is a flexible library that plays the role of V in an MVC framework


 
 #### 2. What are "smart"(logic) and "dumb"(display) components? Explain the difference and also add why we bother to make the distinction between them.
 
 
 //Your Answer
 
 smart(logic) components are components that hold and manage state. Smart components carry out most of the logic and pass props to dumb components.
 dumb(display) components are components without state. Dumb components are primarily used for presentation. 
 
 //Googled Answer
 
 Smart components (or container components) have the burden of being smart. They are the ones that keep track of state and care about how the app works. The container components do the heavy lifting and pass the data down to the presentational components as props.
 
 Dumb components are also called ‘presentational’ components because their only responsibility is to present something to the DOM. Once that is done, the component is done with it.
 
 
#### 3. When we use "yarn add ..." in the terminal - what is yarn doing? And what file will always be automatically updated after we add a package with yarn?
 
 
 //Your Answer
 
 yarn add is used to download a package, such as the react package. 
 
 //Googled Answer
 
 yarn add will automatically add the [package] to your dependencies in your package.json. It will also update your yarn.lock to reflect the change.
 
 
#### 5. There are three mistakes in this code that would cause it to break our application. Find the mistakes and fix them:

import React, { Component } from 'react';

class Recipes extends React.Component {
  constructor(props){
    super(props)
    this.state = {
      recipes: {
        name: 'Meatballs',
        name: 'Mac & Cheese'
      }
    }
  }

  render() {
      
    const { recipes } = this.state
     
    return (

      recipes.map(function(recipe){
        return(
        <ul>
          <li key={recipe.name}>{recipe.name}</li>
        </ul>
        )
      })
    );
  }
}

export default Recipes;

#### 6. Name three html input types. (NOTE: text is the default type - so it doesn't count in this case)
 
 //Your Answer
 
 button
 url
 image
 
 //Googled Answer
 
 button, checkbox, color, date, datetime-local, email, file, hidden, image, month, number, password, radio, range, reset, search, submit, tel, text, time, url, week 
 
 #### 7. How would you explain state to a friend who doesn't know code?
 
 //Your Answer
 
 If you imagine a river... state is what we can change upriver to influence actions and behaviors (rendering) downriver. 
 
 //Googled Answer
 
 If you can change the value on a thermometer, that means you have the ability to put a piece of matter into a different state. With water, simply put it in your freezer (below 32F) and its state will change from liquid to a solid. If you put it on a hot stovetop (above 212F), its state will change from liquid to gas. All of this can be done just by changing one value: its temperature.
 
 #### 8. What is the difference between component state and props? Your answer should include a short explanation of both.
 
 
 //Your Answer
 State is held in one component, preferably as high 'upstream' as possible. State is mutable, and can be updated using setState. setState re-renders the component and all of its child components.
 
 When state is sent from the parent component to children components, this is known as props. Props should not be modified in the children component. 
 
 //Googled Answer
 
  State is referred to the local state of the component which cannot be accessed and modified outside of the component and can only be used & modified inside the component. Props, on the other hand,make components reusable by giving components the ability to receive data from the parent component in the form of props.
  
#### 9. Write a paragraph or so about your experience with building tic-tac-toe. Some topics to start with might be: things you learned about yourself, concepts from React that stood out to you, something about pair programming (if you paired), or the experience of building something in code from scratch.

tic-tac-toe was really hard. I feel like I have a good grasp on React concepts such as state, setState and props. However, I am still having trouble approaching problems and determining the flow. For example, I had no idea what should go in state, or what functions/methods to use and when to use them. I think the one thing I learned about myself is that I need to spend a lot more time on React. Additionally, this was the first time I had a negative experience with mobb programming. One of the members of my group had a really good grasp on React so we moved through the project very quickly. It made it much harder to follow why we were doing what, and when. That being said, it was very rewarding building a usable/working application from scratch.
