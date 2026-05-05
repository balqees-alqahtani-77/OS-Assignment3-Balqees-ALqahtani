# Assignment 3 - Complete Documentation

**Student Name**: [BALQEES ALQAHTANI]  
**Student ID**: [445052134]  
**Date Submitted**: [6 May 2026]

---

## 🎥 VIDEO DEMONSTRATION LINK (REQUIRED)

> **⚠️ IMPORTANT: This section is REQUIRED for grading!**
> 
> Upload your 3-5 minute video to your **PERSONAL Gmail Google Drive** (NOT university email).
> Set sharing to "Anyone with the link can view".
> Test the link in incognito/private mode before submitting.

**Video Link**: [[Paste your personal Gmail Google Drive link here](https://drive.google.com/file/d/1NelVYfZ4BxxDc02YlU-4poj_OuuyJdMK/view?usp=drivesdk)]

**Video filename**: `[445052134]_Assignment3_Synchronization.mp4`

**Verification**:
- [ ] Link is accessible (tested in incognito mode)
- [ ] Video is 3-5 minutes long
- [ ] Video shows code walkthrough and commits
- [ ] Video has clear audio
- [ ] Uploaded to PERSONAL Gmail (not @std.psau.edu.sa)

---

## Part 1: Development Log (1 mark)

Document your development process with **minimum 3 entries** showing progression:

### Entry 1 - Tuesday, April 28, 2026 - 6:00 PM
**What I implemented**: Added ReentrantLock to protect shared variables  

**Challenges encountered**: Race condition issues  

**How I solved it**: Used lock with try-finally  

**Testing approach**: Ran program multiple times  

**Time spent**: 1 hour  

---

### Entry 2 - Thursday, April 30, 2026 - 7:30 PM
**What I implemented**: Protected execution log using lock  

**Challenges encountered**: ConcurrentModificationException  

**How I solved it**: Locked ArrayList during modification  

**Testing approach**: Tested concurrent read/write  

**Time spent**: 1 hour  

---

### Entry 3 - Saturday, May 2, 2026 - 5:00 PM
**What I implemented**: Added Semaphore for CPU control  

**Challenges encountered**: Managing concurrent access  

**How I solved it**: Used binary semaphore  

**Testing approach**: Ran with multiple threads  

**Time spent**: 1 hour

---

### Entry 4 - [Date, Time]
**What I implemented**: 

**Challenges encountered**: 

**How I solved it**: 

**Testing approach**: 

**Time spent**: 

---

### Entry 5 - [Date, Time]
**What I implemented**: 

**Challenges encountered**: 

**How I solved it**: 

**Testing approach**: 

**Time spent**: 

---

## Part 2: Technical Questions (1 mark)

### Question 1: Race Conditions
**Q**: Identify and explain TWO race conditions in the original code. For each:
- What shared resource is affected?
- Why is concurrent access a problem?
- What incorrect behavior could occur?

**Your Answer**:

[Your answer here - 4-6 sentences with code examples]

---

### Question 2: Locks vs Semaphores
**Q**: Explain the difference between ReentrantLock and Semaphore. Where did you use each in your code and why?

**Your Answer**:

[Your answer here - explain your implementation choices]

---

### Question 3: Deadlock Prevention
**Q**: What is deadlock? Explain TWO prevention techniques and what you did to prevent deadlocks in your code.

**Your Answer**:

[Your answer here - reference try-finally blocks, lock ordering, etc.]

---

### Question 4: Lock Granularity Design Decision 
**Q**: For Task 1 (protecting the three counters), explain your lock design choice:
- Did you use ONE lock for all three counters (coarse-grained) OR separate locks for each counter (fine-grained)?
- Explain WHY you made this choice
- What are the trade-offs between the two approaches?
- Given that the three counters are independent, which approach provides better concurrency and why?

**Your Answer**:

[Your answer here - explain coarse-grained vs fine-grained locking, independence of counters, concurrency implications. Show understanding of when to use each approach. 5-8 sentences expected.]

---

## Part 3: Synchronization Analysis (1 mark)

### Critical Section #1: Counter Variables

**Which variables**: 

**Why they need protection**: 

**Synchronization mechanism used**: 

**Code snippet**:
```java
// Paste your implementation here
```

**Justification**: 

---

### Critical Section #2: Execution Log

**What resource**: 

**Why it needs protection**: 

**Synchronization mechanism used**: 

**Code snippet**:
```java
// Paste your implementation here
```

**Justification**: 

---

### Critical Section #3: CPU Semaphore

**Purpose of semaphore**: 

**Number of permits and why**: 

**Where implemented**: 

**Code snippet**:
```java
// Paste your implementation here
```

**Effect on program behavior**: 

---

## Part 4: Testing and Verification (2 marks)

### Test 1: Consistency Check
**What I tested**: Running program multiple times to verify consistent results

**Testing procedure**: 
```bash
# Commands used (run the program at least 5 times)
```

**Results**: 
(Show that running multiple times produces consistent, correct results)

**Why synchronization is necessary**: 
(Explain what race conditions COULD occur without synchronization, even if you didn't observe them. Explain which shared resources need protection and why.)

**Conclusion**: 

---

### Test 2: Exception Testing
**What I tested**: Checking for ConcurrentModificationException
**Testing procedure**: Run program multiple times with threads  

**Results**: Consistent outputs  

**What this proves**: Synchronization works correctly  


---

### Test 3: Correctness Verification

**What I tested**: Verifying correct final values  

**Expected values**: Stable and correct results  

**Actual values**: Matched expected  

**Analysis**: No data inconsistency  


---

### Test 4: Different Scenarios

**Scenario tested**: More processes and different time quantum  

**Purpose**: Check stability under changes  

**Results**: Program remained correct  

**What I learned**: Synchronization handles variations  


---

## Part 5: Reflection and Learning

### What I learned about synchronization:

Synchronization prevents race conditions and ensures correct data sharing.  

Locks and semaphores control thread access.  

Without it, results become unpredictable.  

It improves program stability.  


---

### Real-world applications:

**Example 1**: Bank systems (account balance updates)  

**Example 2**: Operating systems (CPU scheduling)  


---

### How I would explain synchronization to others:

It’s like one key for a room—only one person enters at a time to avoid conflicts.  


---

## Part 6: GitHub Repository Information

**Repository URL**: [your link]  

**Number of commits**: 4  


**Commit messages**:  

1. Set student ID  

2. Added ReentrantLock  

3. Added Semaphore  

4. Completed documentation  


---

## Summary

**Total time spent on assignment**: 3 hours  


**Key takeaways**:  

1. Avoid race conditions  

2. Use locks correctly  

3. Test multiple times  


**Most challenging aspect**: Debugging threads  


**What I'm most proud of**: Correct synchronization implementation

**End of Documentation**
