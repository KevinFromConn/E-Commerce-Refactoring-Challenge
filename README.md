# E-Commerce Refactoring Challenge

This application was built by me for this week's module lesson using Global State, and was refactored for this challenge to use React-Redux instead. I first created a store.js file in the utils folder of the client directory, and imported createStore from "react", I imported the reducers.js file from the same utils folder, and then exported the createStore function, referencing the reducer. From there, I updated App.js to use the new createStore function instead of the old Global State, and I changed the Global State < StoreProvider > tag in the JSX to instead be the < Provider > tag supplied by react-redux. Finally, I went through every component and page which referenced Global State, and refactored it to instead look for useDispatch and useSelector as imported from react-redux. Once all the code was refactored, I ran the application to test its functionality, and everything worked as it had while using Global State.

# Screenshot of Application

![Shop-Shop-Screenshot](https://user-images.githubusercontent.com/83373330/138764904-9574cced-9fd3-4de2-a82d-d0e0078d1527.png)

# Link to Live Application

[Heroku-App](https://blooming-garden-81260.herokuapp.com/)