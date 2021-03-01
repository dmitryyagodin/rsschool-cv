# Dmitry Yagodin
## dmitry.yagodin@gmail.com
## Motivation
I am a junior front-end web developer with background in data analytics, research, and media design. In previous roles I had been using programming for data wrangling, web scraping and data visualizations. I have solid coding experience in Python and JavaScript and look forward to improve my skills in modern full-stack web development with React, Node.js, Express.js, MongoDB (**MERN stack**). 

## Hard skills
- HTML5
- CSS3, SASS, Bootstrap
- JavaScript (ES6), React
- SQL (PostgreSQL, Sqlite)
- Python (numpy, pandas)
- Git
## Experience
### Projects
- WordGame app in plain JavaScript. See it on [GitHub pages](https://dmitryyagodin.github.io/word-game/)
- Random Quote Machine. Try it on [Heroku](https://tweet-a-quote.herokuapp.com/)
### Courses and Certifications
- JavaScript Algorithms and Data Structures [(FreeCodeCamp.org)](https://bit.ly/362GSdt)
- Foundations for Big Data Analysis with SQL [(Coursera, Cloudera)](http://bit.ly/3ixJWTY)
- Web application technologies and Django [(Coursera, U of Michigan)](http://bit.ly/2KFcNcG)
- Python for Everybody [(Coursera, U of Michigan)](http://bit.ly/361pFBs)
- SQL for Data Science [(Coursera, U of California, Davis)](http://bit.ly/2LWFSRg)
- Intro to CS and Programming Using Python [(EdX, MIT)](http://bit.ly/3qGgkXA)
- Visualizing Data with Python [(Coursera, U of Michigan)](http://bit.ly/3sGG3kx)
### Code example
**Snail sort algorithm**
```javascript
snail = function(array) {
    let newArr = [];

    while (array.length > 0) {
      try {
        // copy array's upper row to newArr
        newArr = newArr.concat(array[0]);
        // delete this row from the original array
        array = array.slice(1);
        // move the last items for each of the subarrays from array to newArr
        array.forEach(i => newArr = newArr.concat(i.pop()));
        // reverse the array's bottom row, cut it out and add to newArr 
        newArr = newArr.concat(array.pop().reverse());
        // move the first items for each of the subarrays from array to newArr in a reverse order
        newArr = newArr.concat(array.map(item => item.shift()).reverse());
      }
      // break when array is empty the above methods return an error
      catch(err) { 
          break
      }
    }
    
    return newArr;
}
```

## Education
- PhD in Media and Communications, University of Tampere, Finland
- MA in Journalism (media management), St. Petersburg State University, Russia

## Language skills
- English (C1): professional academic work, including scientific writing, university teaching, conference presentations
- Finnish (B2): fluent, 
- Russian (C2): native
