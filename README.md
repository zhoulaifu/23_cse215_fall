
# CSE215: Foundations of Computer Science (State University of New York, Korea, Fall 2023)

# Course overview

This course is presented by the Computer Science Department at SUNY Korea. It is about discrete mathematics, a fundamental branch essential for a deep understanding of computer science. Topics covered include propositional and predicate logic, number theory, proof techniques, sequences, recursion, functions, relations, and sets.

The course materials, available in this public repository, will be added to over the course of the semester. We'll be adapting materials previously used at SUNY Korea and Stony Brook University for our curriculum.


<a id="org6a7ec5b"></a>

# Course objectives

By the end of the course, students are expected to have:

- The skill to create truth tables for diverse applications, such as verifying the validity of an argument or determining the equivalence of two propositions.
- The preliminary capability to reason with precision and prove certain theorems.
- A basic understanding of mathematical concepts like sequences, functions, and relations.

<a id="orgb048669"></a>

# Prerequisites

AMS 151 or MAT 125 or MAT 131


<a id="orgbb0a69f"></a>

# Textbook

Discrete Mathematics: Introduction to Mathematical Reasoning. Susanna S. Epp. 1st Edition

<a id="org1a0f91c"></a>

# Overall Schedule (All time is on Korean time zone)

Lectures:  TU, TH 12:30  - 13:50, at B207

Recitation: TU 15:30  - 16:25, at B207

Homework due time: 23:59 each Thursday  

Office hours: TU 14:00 - 15:00, TH 15:30 - 16:30  at B424

TA office hours: TBA


Final: Dec 12 Tuesday 12:30 - 15:00 pm at B207
# Zoom (just in case):

<https://stonybrook.zoom.us/j/93553126576?pwd=aDBQN1M2V3BUanpHRUtYd0VZbm5YQT09>


<a id="org20bf8ba"></a>

# Grading: Numerical Score

-   Homework: 20%
-   Midterm1: 25%
-   Midterm2: 25%
-   Final: 30%
-   Students with regular participation or constructive feedback get 0.5% or 1% bonus

Namely, the numerical grade for the course will be calculated as:

```
def numerical_grade(Homework, Midterm1, Midterm2, Final, Bonus):
    return 0.20 * Homework + 0.25 * Midterm1 + 0.25 * Midterm2 + 0.30 * Final + Bonus
```


Assignments submitted after the deadline are typically not acceptable. Should you have a valid reason for a late submission, it is essential to communicate with the course instructor promptly, providing all necessary supporting documents. Please note, once solutions to the homework exercises have been disclosed, no submissions can be accepted under any circumstances.


<a id="orgefb96c0"></a>



# Grading: Letter scores 


### The following algorithm  guarantees that (a) around 50% of students get an A or A-, and (b) students will earn a grade higher than or equivalent to what they would receive with a traditional absolute grading system, barring infrequent boundary situations.


We initiate the grading process by calculating numerical scores for each student and the median of these scores. We then define a cutoff score, denoted by 'c',  which is the minimum of the median score and 90. Letter grades will be allocated based on the following ranges:

- A: Greater than 0.7*c + 30 up to 100
- A-: Greater than 'c' up to 0.7*c + 30
- B+: Greater than 'c - 4' up to 'c'
- B: Greater than 'c - 7' up to 'c - 4'
- B-: Greater than 'c - 10' up to 'c - 7'
- C+: Greater than 'c - 14' up to 'c - 10'
- C: Greater than 'c - 17' up to 'c - 14'
- C-: Greater than 'c - 20' up to 'c - 17'
- D+: Greater than 'c - 24' up to 'c - 20'
- D: Greater than 'c - 27' up to 'c - 24'
- D-: Greater than 'c - 30' up to 'c - 27'
- F: Scores equal to or less than 'c - 30'

Please note that the boundaries for the letter grades are exclusive on the lower end and inclusive on the higher end.

Let's say that the cutoff value 'c' is 85. 

For a letter grade 'B+', the score range is greater than 'c - 4' (85 - 4 = 81) and up to 'c' (85). This means that if a student's score is 81.5, their letter grade would be 'B+'. However, if their score is exactly 81, they would not receive a 'B+', but would instead fall into the B range.

The following Python code implements this grading scheme

```
def get_letter_grade(score, c):
    boundaries = {
        'A':  0.7*c + 30,
        'A-': c,
        'B+': c - 4,
        'B':  c - 7,
        'B-': c - 10,
        'C+': c - 14,
        'C':  c - 17,
        'C-': c - 20,
        'D+': c - 24,
        'D':  c - 27,
        'D-': c - 30,
    }
    
    for grade, boundary in boundaries.items():
        if score > boundary:
            return grade
    return 'F'
```




# Instructor

Zhoulai Fu \<zhoulai dot fu at sunykorea.ac.kr\>  or  \<zhoulai dot fu at stonybrook.edu\>


<a id="orgda07346"></a>

# Teaching assistant

Junhyeong Park \<phjpurpleoob@gmail.com\>

<a id="org24aa011"></a>

# Disability Support Services (DSS) Statement

If you have a physical, psychological, medical or learning disability that may impact your course work, please contact  One-Stop Service Center, Academic Building A201, (82) 32-626-1117. They will determine with you what accommodations, if any, are necessary and appropriate. All information and documentation is confidential.

Students who require assistance during emergency evacuation are encouraged to discuss their needs with instructors and the One-Stop Service Center.


<a id="org1af6e2f"></a>

# Academic integrity

Each student must pursue his or her academic goals honestly and be personally accountable for all submitted work. Representing another person's work as your own is always wrong. Faculty members are required to report any suspected instances of academic dishonesty to the Academic Judiciary Committee or the Department of Academic Affairs, Campus Building A, Room 201, (032) 626-1121.


<a id="org0aaca55"></a>

# Critical incident management

SUNY Korea expects students to respect the rights,
privileges, and property of other people. Faculty are required to report to the Department of Academic Affairs any disruptive behavior that interrupts their ability to teach, compromises the safety of the learning environment, or inhibits students' ability to learn.

