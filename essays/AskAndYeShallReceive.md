---
layout: essay
type: essay
title: "Ask and ye shall receive"
# All dates must be YYYY-MM-DD format!
date: 2023-09-08
published: true
labels:
  - Questions
  - Answers
  - StackOverflow
---
## Oh No, A Bug!

Whether you are a beginner or an advanced learner of coding, you cannot always evade the plaguing of bugs in your code that causes a massive ordeal of revising your code, reading line by line, trialing and error guesses of where or what the bug could be until exhaustion. It is incredibly time consuming, drains your energy and sucks the hopes of building your coding project.

I recall for one particular bug concerning pointers that made me turn up to office hours emotionally charged and handed over my laptop to the professor and just asked him to find the bug. He kindly swiveled the laptop back to me and told me to describe what the problem is. In my frustration, I repeated back to him what the compiler error was showing and the professor restated that I, again, needed to describe what the problem was. 

<Figure>
  <img src="../img/Essay/Frustrated.webp" alt="Being Framed" class="img-fluid">
  <figcaption>Retrieved from https://waypointrecoverycenter.com/learning-deal-frustration-recovery/</figcaption>
</Figure>

Coming down from the rage "high", I realized that I was not being helpful with how I was asking for help. I did not provide a context of what my code was and what was it about pointers that I was finding difficulties with. The audacity for me to hold the expectation that my professor would suddenly know what the bug is was foolish of me and very lazy. 

## The Right Way of Asking for Help

Knowing how to frame your question to ask for help is a skill that helps mitigate further frustration already mounting from when the bug appeared. If you are inadequate in your approach like I did, then be prepared to have an inadequate reply. Learn how to articulate your problem in a clear and concise way so that people know how to structurally solve it. 

Later that afternoon, my professor sent me a message on discord to a link to the Stack Overflow forum where it cleared things up for me greatly in terms of how pointers behave and illustrated how I should have asked my question. 

Here's the [QUESTION](https://stackoverflow.com/questions/55928816/c-iterator-range-using-pointers-to-an-array)

```
Q: C++ Iterator range using pointers to an array

I do not want to pass the size of the array as an index parameter.

For my merge_sort, I want to optimize my parameters using the iterator range concept. I can't seem to figure out how to deference the iterator range and access my array. I can deference to access the indices like low and high in recursive_merge_sort, but there does not seem to be an intuitive way to access the array itself. I've been using this great guide on C++ Pointers and Arrays as a starting point.

My Merge Sort C++11 C++17 question brought this concept to light and I like the idea of using iterator ranges to reduce the number of parameters for my sort.
```
In addition to the question, the person provided their code fragment with comments showing possible indications of where the error could be occurring. 

Here the person clearly states what their objectives are and where they are finding problems. The objective is to optimize parameters using iterators and the problem is dereferencing the iterator. There is a mention that the person has consulted textbooks and references a previous related question posted to the same that has been of help in trying to tackle the problem, demonstrating initiative from the asker that they have made an effort. 

The responses to the above questions explained the relationship between pointers, iterators and c++ arrays and provided code examples to display the usages of pointers like iterators like the begin/end iterators. Some responses cautioned the method of passing in an array by pointer and gave potential complications down the road from said method. 

Observing how well the question was posed and how well structured and balanced the responses was, it is then advantageous for the asker as the bug in their code could become more obvious. 

## The Huh Wat Way of Asking for Help.

Hmmm, my embarassing story of my office hour situation should serve as a model of what not to ask. Yet, to solidify and contrast, let us look at this [QUESTION](https://stackoverflow.com/questions/31768272/what-is-the-point-of-using-references-and-pointers-in-c)

```
Q: What is the point of using references and pointers in C++?
I read this similar question but after a few weeks of studying C++ one thing I am curious about is: Why use pointers or references in C++?

Not even why use one over the other, but just why not use the original value?

By default things are passed by value in C++ wouldn't a lot of the confusion and accidental side effects would be removed if the original value were always passed?

Is it simply so that a smaller value can be passed on the stack?
```
This question lacks to show a specific coding problem or challenge that the asker is facing. Hence there is no definitive answer nor a specific solution that can be afforded. While, it asks on the topic of pointers and references, it is too broad and that poses a problem because it leaves a lot for interpretation, gathering varied responses that leads the asker astray. Also, as the question is broad, it would be annoying for responders to have to write lengthy answers to cover all the possible angles of the question. These sentiments are also shared in the replies to the question.


## Is there a perfect question?

<Figure>
  <img src="../img/Essay/AskingQuestions.jpeg" alt="Being Framed" class="img-fluid">
  <figcaption>Retrieved from https://hatrabbits.com/en/asking-questions/</figcaption>
</Figure>

There is no perfect question but there are ways you can perfect it. Okay, I was trying to be philosophical there but in practicality, as you embark on asking questions on a forum like stack overflow, take time to craft your question. Do not just spontaneously garble your question on there (like I did to my professor, although thankfully he was kind enough to have guided me. Imagine the responses I would have gotten had I posted!). With quality questions breeds quality solutions that preserves quality time! A final advice is to listen to feedback as these serve as stepping stones to better-ing questions next time!
