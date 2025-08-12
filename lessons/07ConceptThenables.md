# ## Concept: Thenables

## Overview

No overview provided

## Learning Objectives

Learning objectives will be defined as the lesson progresses.

## Topics Covered

Topics will be covered as the lesson progresses.

## Status

pending

## Assignment

Assignment for Lesson 7

### Objective

No objective specified

### Expected Capabilities

Expected capabilities will be defined as the lesson progresses.

### Instructions

Instructions will be provided when the lesson is generated.

### Tasks

#### Task 1: Task 1

Continue to work in the `node-express-course` repository. Create a new branch, `week7`. **This should be created when the `week6` branch is active, so that your new work adds to the previous work.** You will work in the directory `04-store-api/starter`. Once you have changed to that directory, be sure to run `npm install` to install the required Node modules. As in previous lessons, you will duplicate the work of the instructor, testing as you go with Postman.

**This is a difficult lesson, so take your time with it**, stopping the video as needed so that you understand what is being done. Also, if you get stuck, the instructor’s solution is in the `04-store-api/final` directory. The idea is that one can search by any or all of these attributes: `featured`, `name`, `price`, `rating`, and `company`. For the numeric fields (`price` and `rating`), one can also specify that you are comparing the number given to see if its “greater than”, “less than”, or “equal to” that value. One can also specify a sort order (ascending or descending). Also, one can specify a `skip` and a `limit`, to facilitate pagination through the result. Be sure that you test each step with Postman. Almost all the work will be done in the `controllers/product.js` file. That file has two methods, `getAllProducts` and `getAllProductsStatic`. The `getAllProductsStatic` method is there for you to experiment with and won’t be directly reviewed.

```

```

### Submission Instructions

Please submit on time

### Checklist

Checklist will be provided when the lesson is generated.

### Check for Understanding

Understanding checks will be provided when the lesson is generated.

## Subsections

### ## Concept: Thenables

In this lesson, you parse the query parameters passed with the REST request, appending the search filters that result to your find operation. As in the previous lesson, you communicate with a MongoDB database. The lesson starts at 3:07:00 of **[this video](https://www.youtube.com/watch?v=rltfdjcXjmk&t=11220)**, and continues to 5:05:34.

### Concept: Thenables

One part of this assignment is a little confusing. You will see code like this:

```javascript
let result = Product.find(queryObject);
...
result = result.sort(sortList);
...
result = result.select(fieldsList);
...
const products = await result;
```

How can this work? Isn’t `Product.find` asynchronous? The reason it works is that `Product.find` doesn’t return a `Promise`. It returns something that works like a Promise, but has extended capabilities. This is called a “then-able”. In this case, the thenable allows the search to be further defined. The `Product.find` call does not immediately send anything to the Mongo database, until `await` (or `.then`) is called on the thenable. Only then is the fully qualified search is sent to the database, and the Promise is resolved, and the products found by the search are returned.

### Concept: Regular Expressions

Regular expressions provide a general purpose string parsing syntax. A regular expression can be used to identify strings that match a pattern. Regular expressions can also be used to create modified strings by substituting character patterns. There are several tutorials on regular expressions on the web. Here is a selection of them:

* [Regex Tutorial](https://regexlearn.com/)
* [Game to help learn regex](http://play.inginf.units.it/#/)
* [Interactive regex exercises](https://regexone.com/)

In this course, we will not teach the use of regular expressions, but you should be aware of their purpose. To complete your homework, you can just copy the regular expressions used by the instructor from their location in the final directory.

**Video URL:** No video available

**Code Examples:**

No code examples available

**External Links:**

No external links available

**Quizzes:**

No quizzes available

## Supplemental Videos

No supplemental videos available

## References

No references available

## Podcast URL

No podcast available