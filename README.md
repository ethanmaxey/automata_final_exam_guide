# 🤖 Automata Final Study Guide

### New Questions
Q9. Let L1 and L2 be arbitrary languages, subject to the specification in either (i) or (ii). Conisder the following questions: Q1, Q2.... etc 

## 🔎 Question Navigation

- [Question 1](#question-1)
- [Question 2](#question-2)
- [Question 3](#question-3)
- [Question 4](#question-4)
- [Question 5](#question-5)
- [Question 6](#question-6)
- [Question 7](#question-7)
- [Question 8](#question-8)
- [Question 9](#question-9)

## Question 1

> Also from Exam 1 Question 4 (14/20)

> Construct a regulat expression over {a, b, c} for the language accepted by this nfa:

$$
\text{Summer 2022}\\quad
$$

Over {a, b, c}

|               | a      | b      | c      |         |
| ------------- |:------:|:------:|:------:|:-------:|
| **A**         | B      | /      | /      |    0    |
| **B**         | C      | /      | A      |    1    |
| **C**         | /      | A, B   | /      |    0    |




## Question 2

> Also from Exam 2 Question 1 (20/20)

> Prove that the language L(G) is not regular where G is the following cfg: G = {...}. Note: You must first determine L(G)

$$
\text{Summer 2022}\\quad
$$

G = ({S,A,B}, {a,b,c}, {S->Abb|b, A->aaS, B->c}, S). 

## Question 3

> Also from Exam 2 Question 3 (15/30)

> Construct a reduced dfa for the following extended regular expresion over {..}: Note: You must first determine nfas for the simple regular expressions the handle the logic operator (intersection). The answer must then be reduced.

- Use https://cyberzhg.github.io/toolbox/nfa2dfa/ to help convert regex to nfa.
- Use https://aswaddev.github.io/dfa-minimizer/ to reduce your final DFA

$$
\text{Summer 2022 \quad over (0, 1)}\\quad
$$

[(10*)* ∩ ¬(0*10*)]

## Question 4

> Also from Exam 2 Question 4 (4.5/15)

> Construct a Chomsky normal form grammar for L(G) for the following cfg G: G = {...} Note: You must first remove all epsilon and unit productions.

Removal of epsilon productions video: https://www.youtube.com/watch?v=mlXYQ8ug2v4

$$
\text{Summer 2022}\\quad
$$

G = ({S,B}, {a,b,c,d}, {S->bSb|Ba, B->BdSc|S|ε}, S). 

## Question 5

> Also from Exam 2 Question 5 (4/25)

> Construct a Greibach normal form grammar for L(G) for the following cfg G: G = {...} Note: You must first remove all unit productions. You must derive all the productions for S and A; indicate how the result looks for S' and A'.

$$
\text{Summer 2022}\\quad
$$

G = ({S,A}, {a,b}, {S->AS|A, A->SA|ab}, S). 

## Question 6

> Also from Exam 3 Question 1

> Prove that the following language L is not context-free. L = {..} 

$$
\text{Summer 2022}\\quad
L = [a^{n+2} b^{n+1} b^n \quad \text{|}\  n\geq 0]
$$

- Leiss on Pumping Lemma (0:00 - 12:28) [[Video](https://www.youtube.com/watch?v=VVbsZKxvLM8)]

- Pumping Lemma (For CFL) 📹 [[Video](https://www.youtube.com/watch?v=jRhqx1_KcCk)]
- Example 1 📹 [[Video](https://youtu.be/eQ0XkUk3qGk)]
- Example 2 📹 [[Video](https://youtu.be/DPs8sBcIjs8)]

## Question 7

> Also from Exam 1 Question 2 (23/23)

> Consider the class {class} of all CFL whose words are ... over ... . (a) Is {class} countable? (b) Is the class {not class} countable where it consists of all languages over {..} that are not context free? (c) Is the class {..} intersection {...} countable? For each question, you must give a precise argument substantiating your answer.

$$
\text{Summer 2022}\\quad
$$

class = {EVENCFa}

## Question 8

> Also from Exam 3 Question 5

> Construct a Turing machine for the language in Question 1. L = {...}. Describe first in words what you are doing, then formulate the formal Turing machine.

$$
\text{Summer 2022}\\quad
L = [a^{n+2} b^{n+1} b^n \quad \text{|}\  n\geq 0]
$$

[[Turing Machine Creator Website](https://turingmachine.io/)]

- LEISS (22:00 - 1:25:20) 📹 [[Video](https://www.youtube.com/watch?v=bqQ55-KM_7E)]
- Turing Machines - Leiss Lecturing 📹 [[Video](https://www.youtube.com/watch?v=bqQ55-KM_7E)]

## Question 9

> Let L1 and L2 be arbitrary languages, subject to the specification in either (i) or (ii). Consider the four questions: (Q1) Does L2 - L1 conatin a given fixed word w? (Q2) Is L2 - L1 not empty? (Q3) Does L1 intersect L2 contain a given fixed word w? (Q4) Is L1 intersect L2 not empty? For each of these four questions, explain with reasons whether the general problem is recursive, not recursive but r. e, or non-re. e., provided (i) Both L1 and L2 are recursive (ii) L1 is recursive and L2 is r. e., but not recursive.
