Download Link: https://assignmentchef.com/product/solved-ucs1411-exercise-7-deadlock-avoidance
<br>
Develop a C program to implement the banker’s algorithm for deadlock avoidance.

<u>Algorithm:</u>

<ol>

 <li>Read the following

  <ol>

   <li>Number of processes.</li>

   <li>Number of resources and number of instances of each resource available.</li>

   <li>Maximum requirement of each process,</li>

   <li>Allocated instances of resources</li>

  </ol></li>

 <li>Determine the need of each process</li>

 <li>Repeat the following till all processes are done.

  <ol>

   <li>Check if request of process i less than or equal to need of that process

    <ol>

     <li>If yes proceed</li>

     <li>Otherwise raise an error condition</li>

    </ol></li>

   <li>Check if request of process i less than or equal to available instances

    <ol>

     <li>If yes proceed ii. Otherwise wait till available.</li>

    </ol></li>

   <li>Update the available vector, allocation vector and need vector</li>

   <li>Generate safety sequence by running safety algorithm.</li>

  </ol></li>

</ol>

SAMPLE INPUT &amp; OUTPUT:

Banker’s Algorithm

<ol>

 <li>Read Data</li>

 <li>Print Data</li>

 <li>Safety Sequence 4. Exit</li>

</ol>

Enter the option :1

Number of processes: 5 P0, P1, P2, P3, P4

Number of resources: 3 A B C

Number of Available instances of A: 3 Number of Available instances of B: 3

Number of Available instances of C: 2

Maximum requirement for P0: 7 5 3

Maximum requirement for P1: 3 2 2

Maximum requirement for P2: 9 0 2

Maximum requirement for P3: 2 2 2

Maximum requirement for P4: 4 3 3

Allocated instances to P0: 0 1 0

Allocated instances to P1: 2 0 0

Allocated instances to P2: 3 0 2

Allocated instances to P3: 2 1 1

Allocated instances to P4: 0 0 2

Enter the option: 2

Alloc Max Need Avail

A B C A B C A B C A B C

P0 0 1 0 7 5 3 * * * 3 3 2

P1 2 0 0 3 2 2 * * *

P2 3 0 2 9 0 2 * * *

P3 2 1 1 2 2 2 * * *

P4 0 0 2 4 3 3 * * *

Enter the option: 3 Display the Safety Sequence:

* * * * *

Enter the option: 4