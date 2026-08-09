# Network Lab Experiment
# NETWORK LAB EXPERIMENTS – TCP SOCKET PROGRAMMING

---

# QUESTION 1 – BASIC TCP CLIENT-SERVER COMMUNICATION

## Aim

To develop a TCP client-server application using socket programming where the client sends a message to the server and the server sends a reply back to the client.

## Commands Used

```bash
cd /mnt/c/Users/hp/Desktop/tcp
nano server.c
gcc server.c -o server
./server
```

In the second terminal:

```bash
cd /mnt/c/Users/hp/Desktop/tcp
nano client.c
gcc client.c -o client
./client
```

## Procedure

1. Open Ubuntu/WSL terminal.
2. Navigate to the TCP project folder.
3. Create and save `server.c`.
4. Compile the server using `gcc server.c -o server`.
5. Run the server using `./server`.
6. Open a second terminal.
7. Navigate to the same TCP folder.
8. Create and save `client.c`.
9. Compile the client using `gcc client.c -o client`.
10. Run the client using `./client`.
11. The client establishes a TCP connection with the server.
12. The client sends the message `Hello Server`.
13. The server receives the message.
14. The server sends `Hello Client` as the reply.
15. The client displays the reply.
16. Both sockets are closed.

## Output

### Server Output

```text
Socket Created Successfully...
Bind Successful...
Waiting for Client...
Client Connected...
Client Says: Hello Server
Reply Sent...
Connection Closed...
```

### Client Output

```text
Socket Created Successfully...
Connected to Server...
Message Sent: Hello Server
Reply from Server: Hello Client
Connection Closed...
```

## Conclusion

Thus, a TCP client-server application was successfully implemented using socket programming, and communication between the client and server was established successfully.

---

# QUESTION 2 – ARITHMETIC SERVER

## Aim

To develop a TCP client-server application where the client sends two integers to the server and the server performs addition, subtraction, multiplication, and division.

## Commands Used

```bash
cd /mnt/c/Users/hp/Desktop/tcp
nano arithmetic_server.c
gcc arithmetic_server.c -o arithmetic_server
./arithmetic_server
```

In the second terminal:

```bash
cd /mnt/c/Users/hp/Desktop/tcp
nano arithmetic_client.c
gcc arithmetic_client.c -o arithmetic_client
./arithmetic_client
```

## Procedure

1. Open Ubuntu/WSL terminal.
2. Navigate to the TCP project folder.
3. Create and save `arithmetic_server.c`.
4. Compile and run the arithmetic server.
5. Open a second terminal.
6. Create and save `arithmetic_client.c`.
7. Compile and run the arithmetic client.
8. Enter two integers in the client.
9. The client sends both integers to the server.
10. The server performs addition, subtraction, multiplication, and division.
11. The server sends all results to the client.
12. The client displays the received results.
13. The connection is closed.

## Output

### Server Output

```text
Socket Created Successfully...
Bind Successful...
Waiting for Client...
Client Connected...
Results Sent Successfully...
Connection Closed...
```

### Client Output

```text
Socket Created Successfully...
Connected to Server...
Enter first integer: 25
Enter second integer: 35
Numbers Sent Successfully...

Addition = 60.00
Subtraction = -10.00
Multiplication = 875.00
Division = 0.71
Connection Closed...
```

## Conclusion

Thus, a TCP arithmetic server was successfully implemented to perform arithmetic operations on two integers received from the client.

---

# QUESTION 3 – STRING PROCESSING SERVER

## Aim

To develop a TCP client-server application where the client sends a string to the server and the server finds its length, converts it to uppercase, and reverses it.

## Commands Used

```bash
cd /mnt/c/Users/hp/Desktop/tcp
nano string_server.c
gcc string_server.c -o string_server
./string_server
```

In the second terminal:

```bash
cd /mnt/c/Users/hp/Desktop/tcp
nano string_client.c
gcc string_client.c -o string_client
./string_client
```

## Procedure

1. Open Ubuntu/WSL terminal.
2. Navigate to the TCP project folder.
3. Create and save `string_server.c`.
4. Compile and run the string server.
5. Open a second terminal.
6. Create and save `string_client.c`.
7. Compile and run the string client.
8. Enter the string `Computer Networks`.
9. The client sends the string to the server.
10. The server calculates the length of the string.
11. The server converts the string to uppercase.
12. The server reverses the string.
13. The server sends the processed results to the client.
14. The client displays all the results.
15. The connection is closed.

## Output

### Input

```text
Computer Networks
```

### Server Output

```text
Socket Created Successfully...
Bind Successful...
Waiting for Client...
Client Connected...
Received String: Computer Networks
Results Sent Successfully...
Connection Closed...
```

### Client Output

```text
Socket Created Successfully...
Connected to Server...
Enter a string: Computer Networks
String Sent Successfully...

String Length = 17
Uppercase = COMPUTER NETWORKS
Reversed = skrowteN retupmoC
Connection Closed...
```

## Conclusion

Thus, a TCP string processing server was successfully implemented to find the length, convert the string to uppercase, and reverse the string received from the client.

---

# QUESTION 4 – ARRAY PROCESSING SERVER

## Aim

To develop a TCP client-server application where the client sends N integers to the server and the server calculates the sum, average, maximum element, and minimum element.

## Commands Used

```bash
cd /mnt/c/Users/hp/Desktop/tcp
nano array_server.c
gcc array_server.c -o array_server
./array_server
```

In the second terminal:

```bash
cd /mnt/c/Users/hp/Desktop/tcp
nano array_client.c
gcc array_client.c -o array_client
./array_client
```

## Procedure

1. Open Ubuntu/WSL terminal.
2. Navigate to the TCP project folder.
3. Create and save `array_server.c`.
4. Compile and run the array server.
5. Open a second terminal.
6. Create and save `array_client.c`.
7. Compile and run the array client.
8. Enter the number of elements as `6`.
9. Enter the array elements `2 4 6 8 10 12`.
10. The client sends the array to the server.
11. The server calculates the sum.
12. The server calculates the average.
13. The server finds the maximum element.
14. The server finds the minimum element.
15. The server sends the results to the client.
16. The client displays the results.
17. The connection is closed.

## Output

### Input

```text
2 4 6 8 10 12
```

### Server Output

```text
Socket Created Successfully...
Bind Successful...
Waiting for Client...
Client Connected...
Received 6 integers:
2 4 6 8 10 12
Results Sent Successfully...
Connection Closed...
```

### Client Output

```text
Socket Created Successfully...
Connected to Server...
Enter number of elements: 6
Enter 6 integers:
2 4 6 8 10 12
Array Sent Successfully...

Sum = 42
Average = 7.00
Maximum Element = 12
Minimum Element = 2
Connection Closed...
```

## Conclusion

Thus, a TCP array processing server was successfully implemented to calculate the sum, average, maximum, and minimum elements of an array received from the client.

---

# QUESTION 5 – MATRIX ANALYZER

## Aim

To develop a TCP client-server application where the client sends a square matrix to the server and the server determines its type, calculates the sum of its elements, and calculates its trace.

## Commands Used

```bash
cd /mnt/c/Users/hp/Desktop/tcp
nano matrix_server.c
gcc matrix_server.c -o matrix_server
./matrix_server
```

In the second terminal:

```bash
cd /mnt/c/Users/hp/Desktop/tcp
nano matrix_client.c
gcc matrix_client.c -o matrix_client
./matrix_client
```

## Procedure

1. Open Ubuntu/WSL terminal.
2. Navigate to the TCP project folder.
3. Create and save `matrix_server.c`.
4. Compile and run the matrix server.
5. Open a second terminal.
6. Create and save `matrix_client.c`.
7. Compile and run the matrix client.
8. Enter the order of the square matrix as `3`.
9. Enter the matrix elements.
10. The client sends the matrix to the server.
11. The server determines the matrix type.
12. The server calculates the sum of all matrix elements.
13. The server calculates the trace of the matrix.
14. The server sends the results to the client.
15. The client displays the results.
16. The connection is closed.

## Output

### Input Matrix

```text
1 2 3
0 4 5
0 0 6
```

### Server Output

```text
Socket Created Successfully...
Bind Successful...
Waiting for Client...
Client Connected...
Received Matrix of Order 3:
1 2 3
0 4 5
0 0 6
Results Sent Successfully...
Connection Closed...
```

### Client Output

```text
Socket Created Successfully...
Connected to Server...
Enter order of square matrix: 3
Enter 3 x 3 matrix elements:
1 2 3
0 4 5
0 0 6
Matrix Sent Successfully...

Matrix Type = Upper Triangular Matrix
Sum of Matrix Elements = 21
Trace of Matrix = 11
Connection Closed...
```

## Conclusion

Thus, a TCP matrix analyzer was successfully implemented to determine the matrix type, calculate the sum of matrix elements, and calculate the trace of a square matrix.



