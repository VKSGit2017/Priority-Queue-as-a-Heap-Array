# Priority-Queue-as-a-Heap-Array
Builds a proiority queue as a heap stored in an array, dequeue the next proiority item &amp; maintain the heap

CSCI-2270
Assignment 7
Instructor: Boese
Priority Queue as a Heap Array
Emergency Room Patient Admittance
Objectives
• Build a priority queue as a heap stored in an array
• Dequeue the next priority item and maintaining the heap
For this assignment, you will be implementing a class of your own: a priority queue,
which is a variation on the standard queue. The standard queue processes element
in the first-in, first-out ("FIFO") manner typical of ordinary waiting lines. Queues can
be handy, but a FIFO strategy isn't always what's needed. A hospital emergency
room, for example, needs to schedule patients according to priority. A patient with a
more critical problem will pre-empt others even if they have been waiting longer.
This is a priority queue, where elements are prioritized relative to each other and
when asked to dequeue one, it is the highest priority element in the queue that is
removed.
The priority queue will store a collection of structs that keep track of the patient
name and an integer for the priority. Smaller integers are considered higher priority
than larger ones and are dequeued ahead of larger values.
The header file is provided with a struct to maintain the patient information and a
class to maintain the priority queue. In this example, assume all priority numbers
are unique (in a real ER program, the numbers may be from 1 to 10 plus the date/time
stamp to determine who came in first when multiple have the same priority).
Specifications
• Use the provided header file – do not change in any way!
• Test your program with the provided driver program – without changing the
driver program your output should match what is provided below.
Submitting Your Code:
Submit your assignment named PriorityQueue.cpp as a zipped file named
HW7_[Firstname]_[Lastname].zip to Moodle.
Expected Output
From the provided driver program, your output should appear as follows:
Adding 22 Lila
===
Patients Waiting
[22] Lila
===
Processing 22 Lila
===
NEXT! - Lila
===
Patients Waiting
No one waiting!
===
Adding 3 Liz
===
Patients Waiting
[3] Liz
===
Adding 19 Xylo
===
Patients Waiting
[3] Liz
[19] Xylo
===
Adding 20 Zedder
===
Patients Waiting
[3] Liz
[19] Xylo
[20] Zedder
===
Adding 15 Ratner
===
Patients Waiting
[3] Liz
[15] Ratner
[20] Zedder
[19] Xylo
===
Adding 7 Tattle
===
Patients Waiting
[3] Liz
[7] Tattle
[20] Zedder
[19] Xylo
[15] Ratner
===
Adding 6 Sassy
===
Patients Waiting
[3] Liz
[7] Tattle
[6] Sassy
[19] Xylo
[15] Ratner
[20] Zedder
===
Adding 2 Elle
===
Patients Waiting
[2] Elle
[7] Tattle
[3] Liz
[19] Xylo
[15] Ratner
[20] Zedder
[6] Sassy
===
Adding 1 Alph
===
Patients Waiting
[1] Alph
[2] Elle
[3] Liz
[7] Tattle
[15] Ratner
[20] Zedder
[6] Sassy
[19] Xylo
===
Adding 5 Ophra
===
Patients Waiting
[1] Alph
[2] Elle
[3] Liz
[5] Ophra
[15] Ratner
[20] Zedder
[6] Sassy
[19] Xylo
[7] Tattle
===
Adding 4 Mommy
===
Patients Waiting
[1] Alph
[2] Elle
[3] Liz
[5] Ophra
[4] Mommy
[20] Zedder
[6] Sassy
[19] Xylo
[7] Tattle
[15] Ratner
===
Processing 1 Alph
===
NEXT! - Alph
9 patients currently waiting.
Adding 1 Aso
===
Patients Waiting
[1] Aso
[2] Elle
[3] Liz
[5] Ophra
[4] Mommy
[20] Zedder
[6] Sassy
[19] Xylo
[7] Tattle
[15] Ratner
===
Adding 8 Vinnie
===
Patients Waiting
[1] Aso
[2] Elle
[3] Liz
[5] Ophra
[4] Mommy
[20] Zedder
[6] Sassy
[19] Xylo
[7] Tattle
[15] Ratner
[8] Vinnie
===
We're CLOSING! Deleting patient queue!
Removing Aso from the queue.
Removing Elle from the queue.
Removing Liz from the queue.
Removing Ophra from the queue.
Removing Mommy from the queue.
Removing Zedder from the queue.
Removing Sassy from the queue.
Removing Xylo from the queue.
Removing Tattle from the queue.
Removing Ratner from the queue.
Removing Vinnie from the queue.
