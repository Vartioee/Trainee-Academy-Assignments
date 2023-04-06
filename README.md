# Eemeli Vartio's Exercise Portfolio
This repository showcases a few of my solutions to the assignments I have done in Trainee Academy. I have chosen assignments that I thought were educational and interesting. They represent a variety of programming concepts we have learned and that I feel I am now using confidently.
# Assignment 1: Grades

**Instructions for the assignment**

We have the following list of students:
```js
const students = [ { name: "Sami", score: 24.75 },
                   { name: "Heidi", score: 20.25 },
                   { name: "Jyrki", score: 27.5 },
                   { name: "Helinä", score: 26.0 },
                   { name: "Maria", score: 17.0 },
                   { name: "Yrjö", score: 14.5  } ];
```
Create a function ```getGrades``` that takes a list of students as a parameter and returns the students' grades in a new array.
Scores are converted to grades in the following way:

```< 14.0 results in grade 0
[14.0, 17.0] results in grade 1
]17.0, 20.0] results in grade 2
]20.0, 23.0] results in grade 3
]23.0, 26.0] results in grade 4

26.0 results in grade 5
```


*Note* the inclusive/exclusive bounds! For example, the range [14.0, 17.0] includes both 14.0 and 17.0, while the range ]17.0, 20.0] excludes 17.0 (but includes everything that is just above 17.0, even 17.000001).

EXTRA: Instead of returning only an array of grade numbers, return an array of new objects, where each object contains the student's name and their grade.

**My implementation**

In this task I need to make a new array with existing data from *students*, convert *scores* to *grades* and print out the new array without the *score* property.

First I made the function and diceded to use ```array.map()``` for solving this task. 
```js
function getGrades (x) {
    x.map(student => {
    }
)}; 
```

Then I made the conditions. Making sure that I get the score ranges right.
```js
if(student.score < 14.0) {
            student.grade = 0;
        }
        if(student.score > 14.0 && student.score <= 17.0) {
            student.grade = 1;
        }
        if(student.score > 17.0 && student.score <= 20.0) {
            student.grade = 2;
        }
        if(student.score > 20.0 && student.score <= 23.0) {
            student.grade = 3;
        }
        if(student.score > 23.0 && student.score <= 26.0) {
            student.grade = 4;
        }
        if(student.score > 26.0) {
            student.grade = 5;
        }
```

Then I just needed to ```return``` my answer and get rid of scores.

*Full code*
```js
const students = [ { name: "Sami", score: 24.75 },
                   { name: "Heidi", score: 20.25 },
                   { name: "Jyrki", score: 27.5 },
                   { name: "Helinä", score: 26.0 },
                   { name: "Maria", score: 17.0 },
                   { name: "Yrjö", score: 14.5  } 
];
function getGrades (x) {
    x.map(student => {
        if(student.score < 14.0) {
            student.grade = 0;
        }
        if(student.score > 14.0 && student.score <= 17.0) {
            student.grade = 1;
        }
        if(student.score > 17.0 && student.score <= 20.0) {
            student.grade = 2;
        }
        if(student.score > 20.0 && student.score <= 23.0) {
            student.grade = 3;
        }
        if(student.score > 23.0 && student.score <= 26.0) {
            student.grade = 4;
        }
        if(student.score > 26.0) {
            student.grade = 5;
        }
        delete student.score;
    });

    return x;
}

console.log(getGrades(students));
```

# Assignment 2
*Instructions for the assignment*
**Selitys**

```js
"Koodia"
```
**Selitys**

```js
"Koodia"
```

**Selitys**

```js
"Koodia"
```
# Assignment 3

*Instructions for the assignment*

**Selitys**

```js
"Koodia"
```

**Selitys**

```js
"Koodia"
```

**Selitys**

```js
"Koodia"
```
