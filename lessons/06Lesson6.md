# Lesson 6

## Overview

No overview provided

## Learning Objectives

Learning objectives will be defined as the lesson progresses.

## Topics Covered

Topics will be covered as the lesson progresses.

## Status

pending

## Assignment

Assignment for Lesson 6

### Objective

No objective specified

### Expected Capabilities

Expected capabilities will be defined as the lesson progresses.

### Instructions

Instructions will be provided when the lesson is generated.

### Tasks

#### Task 1: Task 1

Create a new git branch called `week6`. **This should be created when the `week5` branch is active, so that it adds to week 5’s work.** If you’ve made any changes to the `week5` branch due to reviews on your PR, make sure to update your `week6` branch by following the instructions from [Lesson 4](./ctd-node-lesson-4.md) Continue to work in the `node-express-course/03-task-manager/starter` directory. You duplicate the work of the instructor in the video.

### Additional Assignment

Create a file in the starter directory called `QuizAnswers2.txt`. Put answers to the following questions in it.

1. In this lesson, you created a middleware function called `asyncWrapper`. Why?
2. Suppose that you want to make sure that both a status code and an error message are sent back to the user when they request the URL for a task that does not exist. Assume that you’ve created a `CustomAPIError` class and an error handler that references that class. Complete the code:  
```javascript  
const getTask = asyncWrapper(async (req, res, next) => {  
  const { id: taskID } = req.params;  
  const task = await Task.findOne({ _id: taskID });  
  if (!task) {  
    // your code here  
  }  
  res.status(200).json({ task });  
});  
```

As you will see in the lessons that follow, you do not have to always create the `asyncWrapper` middleware, because you can instead use an NPM package called `express-async-errors` that provides the same capability.

```

```

### Submission Instructions

Please submit on time

### Checklist

Checklist will be provided when the lesson is generated.

### Check for Understanding

Understanding checks will be provided when the lesson is generated.

## Subsections

### Lesson 6

This week begins at 1:29 of **[this video](https://www.youtube.com/watch?v=rltfdjcXjmk&t=5280s)**, and continues until the end of the task manager project, at 3:07:18 of the video.

In this lesson you will continue to develop the Task Manager API, testing with Postman as you go. You will add:

* Input Validation
* Error Handling
* Additional CRUD Operations

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