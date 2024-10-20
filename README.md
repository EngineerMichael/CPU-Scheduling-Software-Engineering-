# Round Robin CPU Scheduling Algorithm

Name: Michael Bonilla 
## Project Scope

The goal of the project is implementation of  the Round Robin algorithm with different time quantum in order to demonstrate how much CPU resources can be used and how process will be executed according to different time quantum.

## Setup

The program is made in Python 2.7, in order to run make sure that Python is installed. The program can be ran through either an IDE or command line. Make sure you have proper Python version installed otherwise there will be errors.

## Input

The input is a csv file that has a format like below and time quantum. Pic below is just an example of what the csv file should look like. 

| Process ID | Arrival Time | Burst Time |
| :--------- | :----------: | ---------: |
| 1          |      0       |          5 |
| 2          |      1       |          7 |
| 3          |      2       |          9 |

## Execution

Open the terminal, run ``` cd RoundRobin ```, and run the command below. Make sure that you add the path to the CSV file and the time quantum you would like to use

``` 
#tq = 5 and process.csv is the path
$ python main.py process.csv 5                                 
```

## Output

Adding the process to the process List

| ID:  1 | Burst Time:  5 | Arrival Time:  0 |
| :----- | :------------- | ---------------- |
| ID:  2 | Burst Time: 7  | Arrival Time: 1  |
| ID: 3  | Burst Time: 9  | Arrival Time: 2  |

Simulation

| ID: 1 | Start: 0  | End: 4  | Time Left: 1 |
| :---- | :-------- | ------- | ------------ |
| ID: 2 | Start: 4  | End: 8  | Time Left: 3 |
| ID: 3 | Start: 8  | End: 12 | Time Left: 5 |
| ID: 1 | Start: 12 | End: 13 | Time Left: 0 |
| ID: 2 | Start: 13 | End: 16 | Time Left: 0 |
| ID: 3 | Start: 16 | End: 20 | Time Left: 1 |
| ID: 1 | Start: 20 | End: 21 | Time Left: 0 |

## Next Steps

Implementation of other CPU Scheduling Algorithms:

- First Come First Serve
- Priority Scheduling 
- Short Job First
