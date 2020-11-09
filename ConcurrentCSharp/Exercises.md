# Concurrency in C#: Practicum

This document class activities and exercises are described to be practised in practicums of Concurrency course of Hogeschool Rotterdam.

### Practical notes:
1. The exercises of each week coresponds to some of the source codes available here in Github: https://github.com/afshinamighi/Courses
2. Coresponding C# projects are represented with bold font at each exercise.
3. In each exercise, students are expected to evaluate specified source codes, understand the structures, analyze expected behaviours of the programs (guess and justify the output), and in some cases reproduce the concept in a different context.
4. In some of the exercises, students are asked to share / discuss / explain results of their evaluations. The teacher will determine how results will be shared with other students and/or the teacher.
5. This document will be updated weekly. 



# Week 1: 
Main objectives of this week is to introduce the main concepts and prepare practical tools needed for upcoming weeks.
**Preparation**:
1.	 We will discuss about threads in week 3. Here, just think about a thread as a separate paths of execution that can be executed simultanously with the main program.
2.	 Refresh your C# programming environment: You are expected to be able to write simple console based programs. A set of possible concepts to be used later are: fundamentals (types, conditional statements, loops), defining attributes, methods, public / private / static, arrays, anonymous functions. Implement a simple program: like a counter class that counts until a given number and the main program instantiates an object from this class and prints the final result. The counter class has a state that keeps the latest counting value.


## Exercises:
1. Concurrency in your machine:
	1.	Make a list of parallel/concurrent programs in your computer: (recall that in mac the command [ps -ax] makes a list of currently running processes with PID and the location of the executable programs). Choose a running program (for example PyCharm) and see how many threads are running by the application.
	2.	Open an internet browser with several tabs. Check how many threads are created. Make a list (at least five) of functionalities (tasks) that each thread of execution is responsible to execute. Share your list with the teacher.
2. **SocketClient, SocketServer**: 
	1.	These two projects implement a simple client and server programs in C#. Create a project in your local machine and run both client and server. Check how network communication is working in this simulation. 
	2.	Assume you are asked to simulate multiple clients trying to communicate with the server simultaneously. How would you do that? What would you need? Explain the logic through the provided client code.Is current server implementation able to handle multiple simultaneous clients? If not, what would be your proposal to solve it? Explain the logic through the provided server code.
3. **MergeSort**: One of the challenges in designing a concurrent program is to recognise potential concurrent tasks. 
	1.	Among various sort algorithms one of the well-known ones is named **merge sort** algorithm. Read and understand how this algorithm works. You can use the following sesources: [check here](https://www.hackerearth.com/practice/algorithms/sorting/merge-sort/visualize/) , or [here, just don't forget to choose right settings](https://visualgo.net/bn/sorting?slide=1).
	2. Can you recognise sorting tasks that can be done simultaneously? Share your answer with the teacher. **Note**: In week three you will be asked to implement a concurrent version of this algorithm. Therefore, this exercise is crucial to understand and share your ideas. 