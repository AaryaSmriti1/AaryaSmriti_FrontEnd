This is STEELEYE recruitment assignment (Strictly only for drive purpose can't be used for any other purpose).

# Question 1

The List component in the code renders an unordered list of SingleListItem component, it receives an array of items as prop, and creates a SingleListItem component for each of those items. The SingleListItem component renders a single <li> element and adds a onClick behaviour to it.

# Question 2
One of the major problem here is, the items prop for the List component is set to 'null' intially, rather it should be an empty array, JavaScript is not complaining but typescript will. 
In the line 51, the isSelected prop of SingleListItem component is passed the value as selectedIndex which is of type number, but the isSelected prop is of type boolean. That will be managed by type conversion, but it is not advised to write code like that.

# Question 3
Kindly refer drive.js for editted code (file is present in this repo. only)
