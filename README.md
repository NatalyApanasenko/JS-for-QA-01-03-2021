1) Create object "post" which should contain following key:
title body(string value),
author(string value),
views(number value),
isLive (boolean value),
someFunction(function type) - result of calling console.log('Some value'),
comment: object which contain information about the authot - first name, last name and comment body.


const post = {
    titleBody: 'Photo',
    author: 'Nataly',
    views: 89,
    isLive: 'true',

    someFunction: function () {
        console.log('Some value')
    },
    comment: {
        firstName: 'Nataly',
        lastName: 'Apanasenko',
        commentBody: 'Photograph',
    }
};

// Example
const post = {
titleBody: 'Some cool title',
...
}
1.1 Get "comment body" key and "someFunction" value using dots and bracket notation

1.2 Get the length of post object and write the script which should return the list of the properties values of a "post" object

2. Write the function called "helloColleagues" which should accept two parameter "company" and "team" and should return the string with `I am working in "company" in amazing "team"` - use template string syntax to paramerize string value - ``
