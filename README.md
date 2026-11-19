# CSA09 – Programming in Java – Assignment 3 (CO3)

**Register number:** 192524480  
**Language:** Java (JDK 17 or later recommended)

## Tasks and source files

| Task | Topic | Java source |
|---|---|---|
| Q1 | Bank ATM – exception handling | [ATM.java](Task01/ATM.java) |
| Q2 | Online examination portal – user-defined exceptions and chaining | [ExamPortalDemo.java](Task02/ExamPortalDemo.java) |
| Q3 | Daily sales report – resource safety and try-with-resources | [SalesReport.java](Task03/SalesReport.java) |
| Q4 | Thread creation and life cycle – scanner stations | [ScannerStations.java](Task04/ScannerStations.java) |
| Q5 | Cinema seat booking – synchronization | [SeatBooking.java](Task05/SeatBooking.java) |
| Q6 | Deadlock concepts and producer-consumer token counter | [TokenCounter.java](Task06/TokenCounter.java) |
| Q7 | Concurrent fault-tolerant semester result processor | [ResultProcessor.java](Task07/ResultProcessor.java) |

## Compile and run

Open a terminal in the relevant task folder. Compile and run the class:

```bash
javac FileName.java
java ClassName
```

Examples:

```bash
cd Task02
javac ExamPortalDemo.java
java ExamPortalDemo
```

- **Q1:** Run `ATM` and enter an account number (at least six digits) and a numeric withdrawal amount. To test the card-reader path, create an empty `card-reader.txt` in the same working directory. Try a negative amount, an amount above the balance, and non-numeric input.
- **Q2:** Run `ExamPortalDemo`. It demonstrates exception propagation and preserves the original `IOException` as the cause.
- **Q3:** Run `SalesReport` with optional arguments: input folder and output filename. Example: `java SalesReport stores sales-summary.txt`. If the input folder does not exist, sample store files are created.
- **Q4:** Run `ScannerStations`. Completion order may vary between runs.
- **Q5:** Run `SeatBooking`. The synchronized booking operation should print `Seats sold: 10`.
- **Q6:** Run `TokenCounter`. Expected final line: `Sum of tokens collected: 210 (expected 210)`.
- **Q7:** Run `ResultProcessor` with optional score-file folder and thread-pool size (1, 2, 4 or 8). Example: `java ResultProcessor score-files 4`. If the folder is absent, sample score files are created, including one corrupt file.

## Submission checklist

- Execute every task locally and capture your own output screenshots.
- Add the required test tables, stack traces, logs, timing measurements and graphs from your actual runs.
- For Q4 and Q5, repeat the experiments as specified in the assignment and record the observed results.
- For Q7, measure pool sizes 1, 2, 4 and 8 using the same input set.
- Clearly label Student A and Student B contributions in the joint report. Both students must understand and execute all questions.

**Important:** This repository contains starter implementations of the seven main programs. The assignment also requires analysis, experiments, evidence screenshots and report sections; those must be completed using your own executions. Do not claim measurements or screenshots that you have not produced.
