# Box Model and Flexbox

## About

This is the homework solution for the Box Model and Flexbox topics, based on the task below.

The solution includes only the markup and corresponding CSS styles.

## Task

* Create a repository `goit-markup-hw-03`.
* Clone the already created repository (`goit-markup-hw-03`) and copy files of the previous work to it (from `goit-markup-hw-02`).
* Add styles for elements shape (width, padding, margins, and borders) and content positioning with Flexbox for layout pages of [Homework #3](https://www.figma.com/file/Kr5Q4EVrEAqpOWko4QeEJb/Web-Studio-(Version-4.0)?type=design&node-id=296708-626&t=xehgKGCXNQoohzws-0).
* Configure GitHub Pages and add a link to the Live Page in the GitHub repository header.
* The solution must meet the mentor's acceptance criteria.

### Module objectives

* Understand what a block model is and what it is used for.
* Learn how to configure element geometry.
* Understand how the spacing (margins and padding) of different elements interact.
* Learn about the basic concepts of Flexbox technology.
* Learn how to configure the properties of the flex container and flex elements.
* Configure individual elements using the `:first-child`, `:last-child`, `:not()` and `:nth-child(an + b)` pseudo-classes.

## Task

* Create a repository `goit-markup-hw-03`.
* Clone the already created repository (`goit-markup-hw-03`) and copy files of the previous work to it (from `goit-markup-hw-02`).
* Add styles for elements geometry (width, padding, margins, and borders) and content positioning with Flexbox for layout pages of [Homework #3](https://www.figma.com/file/Kr5Q4EVrEAqpOWko4QeEJb/Web-Studio-(Version-4.0)?type=design&node-id=296708-626&t=xehgKGCXNQoohzws-0).
* Configure GitHub Pages and add a link to the Live Page in the GitHub repository header.
* The solution must meet the mentor's acceptance criteria.

## Useful information and insights

* Use a container for section content

  Add the following properties with corresponding values for the `.container` class to the CSS file:

  ```
    .container { 
      max-width: 
      padding-left:  
      padding-right:  
      margin-left:  
      margin-right:  
  }
  ```

  In an HTML document, wrap content inside each section, as well as the header and footer in a `div`` with the container class.
* Connect modern-normalize (to normalize browsers' default style) using the [link](https://airlock-on-edge.woolf.university/?url=https%3A%2F%2Fcdnjs.com%2Flibraries%2Fmodern-normalize&resourceId=9168ce8c-eb19-4f64-8957-5261bac864ee&studentId=d22df0d2-a53a-49c8-bf11-bc01ca37c314&token=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc1ZlcmlmaWVkIjp0cnVlLCJvcmciOnsiaWQiOiIyODU2YWNkMy1jMWUxLTQyMWMtOTg5ZS1jN2RkYmQzMmIyZjIiLCJncm91cHMiOltdfSwia2luZCI6Im9hdXRoIiwic2NvcGUiOiIqIiwiaXNzIjoidXJuOldvb2xmVW5pdmVyc2l0eTpzZXJ2ZXIvc2VydmljZS9hY2Nlc3MiLCJpZCI6ImQyMmRmMGQyLWE1M2EtNDljOC1iZjExLWJjMDFjYTM3YzMxNCIsImlhdCI6MTY5MjAwNDMxNX0.Gn3pEpWfSHgyGSwOSpsVzUwPeKx1pZVzeK8W9yFr7hk) (use "Copy Link Tag" button).
    
  Link it before project `styles.css` file.
* Use "Visually Hidden" pattern to hide headers. 
  
  Add the following properties for the `.visually-hidden` class to the CSS file:

  ```
  .visually-hidden {
    position: absolute;
    width: 1px;
    height: 1px;
    margin: -1px;
    border: 0;
    padding: 0;
    white-space: nowrap;
    clip-path: inset(100%);
    clip: rect(0 0 0 0);
    overflow: hidden;
  }
  ```
* Set the width / flex-basis of list elements in sections using the `calc()` function:
  ```
    <!-- (the width of the parent element - sum of gaps between elements) / the number of elements in the row -->
    
    .benefits-list-item {
      width: calc((100% - 3 * 24px) / 4);
    }
  ```