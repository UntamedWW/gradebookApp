## Simple JS Grading Helpers

Tiny practice script that calculates a class average, converts numeric scores to letter grades, and prints a pass / fail message for a single student.

### Files

```
gradeHelpers.js   # the functions below
```

### Core functions

| Function                                | Purpose                                                                                             |
| --------------------------------------- | --------------------------------------------------------------------------------------------------- |
| `getAverage(scores)`                    | Returns the arithmetic mean of an array of numbers.                                                 |
| `getGrade(score)`                       | Converts a numeric score to a letter grade (`A++ … F`).                                             |
| `hasPassingGrade(score)`                | Boolean helper – `true` if the grade is not “F”.                                                    |
| `studentMsg(totalScores, studentScore)` | Builds a message showing the class average, the student’s grade, and whether the course was passed. |

### Example run

```js
console.log(
  studentMsg(
    [92, 88, 12, 77, 57, 100, 67, 38, 97, 89], // class scores
    37                                          // student score
  )
);
// → Class average: 72.7. Your grade: F. You failed the course.
```

### Ideas for practice

* Round the average to one decimal place.
* Accept an arbitrary grading scheme via a config object.
* Add colourised console output for pass / fail.
