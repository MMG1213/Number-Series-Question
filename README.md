# Number-Series-Question
🏨 Hilbert's Hotel Room Assigner
Solving Infinity with the Cantor Pairing Function
This Java project demonstrates a mathematical solution to Hilbert's Paradox of the Grand Hotel. It specifically addresses the scenario where an infinite number of buses, each carrying an infinite number of passengers, arrives at a hotel that is already completely full.
🧐 The Problem
In a hotel with an infinite number of rooms (all occupied), how do you accommodate:
An infinite number of new buses?
Each carrying an infinite number of new people?
Without kicking anyone out?
🚀 The Solution: The "Zig-Zag" Method
We cannot simply put Bus 1 in rooms 1 to 
, because Bus 2 would wait forever. Instead, we treat the hotel as a 2D grid and map it to a 1D list of rooms using the Cantor Pairing Function.
The Math
To assign a unique room number (
) to a person based on their Bus ID (
) and Seat ID (
), we use:

This formula ensures that every person gets a unique room number and no rooms are skipped, effectively "flattening" two infinities into one.
💻 How to Use
Clone the repository:
bash
git clone https://github.com
Use code with caution.

Compile the code:
bash
javac HilbertHotelAssigner.java
Use code with caution.

Run the program:
bash
java HilbertHotelAssigner
Use code with caution.

Example Input/Output
Input:
Number of Buses: 2
People per Bus: 2
Output:
text
Bus 0, Seat 1 -> Room 2
Bus 0, Seat 2 -> Room 5
Bus 1, Seat 1 -> Room 4
Bus 1, Seat 2 -> Room 8
Use code with caution.

🛠️ Features
Unique Mapping: Uses the Cantor Pairing Function to prevent double-booking.
Efficient Room Filling: Unlike the Prime Power method, this fills rooms densely to avoid massive gaps.
Scalable: Uses long data types to handle large room assignments.
