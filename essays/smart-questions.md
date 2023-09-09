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
## Ask the question, not the answer

Whether you are a beginner or an advanced learner of coding, you cannot always evade the plaguing of bugs in your code that causes a massive ordeal of revising your code, reading line by line, trialing and error guesses of where or what the bug could be until exhaustion. It is incredibly time consuming, drains your energy and sucks the hopes of building your coding project. I remember the nights when a bug in my code made me want to throw my head into the wall. 

I recall for one particular bug concerning pointers that made me turn up to office hours emotionally charged and handed over my laptop to the professor and just asked him to find the bug. He kindly swiveled the laptop back to me and told me to describe what the problem is. In my frustration, I repeated back to him what the compiler error was showing and the professor restated that I, again, needed to describe what the problem was. 

Coming down from the rage "high", I realized that I was not being helpful with how I was asking for help. I did not provide a context of what my code was and what was it about pointers that I was finding difficulties with. The audacity for me to hold the expectation that my professor would suddenly know what the bug is was foolish of me and very lazy. 

## The right way of asking for help

Knowing how to frame your question to ask for help is a skill that helps mitigate further frustration already mounting from when the bug appeared. If you are inadequate in your approach like I did, then be prepared to have an inadequate reply. Learn how to articulate your problem in a clear and concise way so that people know how to structurally solve it. 

Later that afternoon, my professor sent me a message on discord to a link to the Stack Overflow forum where it cleared things up for me greatly in terms of how pointers differ and showed how I should have asked my question. 

Here's the question

```
Q: What is the difference between const int*, const int * const, and int const *?

I always mess up how to use const int*, const int * const, and int const * correctly. Is there a set of rules defining what you can and cannot do?

I want to know all the do's and all don'ts in terms of assignments, passing to the functions, etc.
```
//I WAS HERE LAST *****


While the heading of his question could be better, it does convey what he’s trying to figure out. Usually something as brief as “python date of previous month” is what other users would enter in as search terms on Google, making it easily found. Another good thing about the question is that it’s not just a question. The asker shows what he or she has done and that he or she has put in some effort to answer the question. And while it may not be as important as the question itself, the asker shows courtesy, which does increase the chance of getting an answer.

```
A: datetime and the datetime.timedelta classes are your friend.

1. find today
2. use that to find the first day of this month.
3. use timedelta to backup a single day, to the last day of the previous month.
4. print the YYYYMM string you're looking for.

Like this:

 >>> import datetime
 >>> today = datetime.date.today()
 >>> first = datetime.date(day=1, month=today.month, year=today.year)
 >>> lastMonth = first - datetime.timedelta(days=1)
 >>> print lastMonth.strftime("%Y%m")
 201202
 >>>

```
 
The asker received six possible answers, and he or she was successful in inciting discussion from multiple users. The answers themselves were clear and were devoid of the rumored sarcasm and hostility of “hackers.” Since I myself have referenced this page and found it useful, I can confidently say that it is a good question.

## The foolproof way to get ignored.

While there are decent questions that benefit everyone, there are those one can ask to create an entirely different effect. In the following example, a user asks how he would, in short, create a desktop application with Facebook.

```
Q: Facebook Desktop Notifier

I am a beginner programmer that have never used anything other than what's included in a language.

I am trying to create a desktop application that notifies me anytime I get an update onfacebook. 
How should go about doing this? Thanks in advance.

edit Sorry I was not clear. Is there any way to make a DESKTOP application with facebook?
```

A simple “yes” would have answered the question, but we know that’s not the sort of answer he or she is looking for. Fortunately, someone kindly responded with a link to Facebook’s developer website. The asker should have done more research on his or her potential project. Then further down the road, he or she could have asked more specific and detailed questions that wouldn’t require a thousand-paged response for a sufficient answer.

## Conclusion

When we rely on others’ generosity and expertise to provide answers to our questions, it should hold that the question we ask should be one that leads to efficient and effective help that not only benefits us, but also the people we ask and others who might ask the same question in the future. Thus, if you have a question… make it a smart one! Asking questions may not always get you the best answer, but asking them in a way that will make others want to answer them will increase the success of finding a good solution and make it a positive experience on all sides.
