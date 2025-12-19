What do I actually want to be capable of designing, explaining, and defending in 14 months?
I want to be capable of everything, solve and create just like that. It should flow in my hands the moment I think about it. 

What kind of engineer do I never want to be again? 
- Someone who can't explain trade-offs
- Someone who panics in design interviews
- Someone gets nervous  by thinking job interview itself

What kind of engineer scares me to become - because of the responsibility it carries?
- Need to be better than ChatGPT or any other LLM
- I am the one who can give better insights and details and in every tiny details

---
### Block A - Big-O & Engineering Thinking

#### Task 1 - Reset your Big-O Mental Model
Big-O as a Language of Trade-offs
1. Why Big-O ignores constants - and when engineers should not ignore them. 
   Reason: When we have larger amount of N which is input, the constants always stays there, it won't show any much difference in the time of execution. So we are ignoring it. 
   We shouldn't ignore when the input is small, those time it will have the impact. 
2. Why O(n log n) is fundamentally different from O(n^2), even if n is small. 
   The reason is almost 1.25 times it's faster in the execution
3. One real-world system where asymptotic analysis alone is misleading. 
   I have no idea on this. Tried to think I didn't get anything
#### Task 2 - Thought Experiment
Question:
You have two implementation of a function:
A: O(n) but with heavy memory allocation
B: O(n log n) but extremely cache-friendly
For n =1 million which might be faster in practice, and why?

Answer: I am going with the option A, the reason it takes memory which RAM we can expand till some extend, but it's N contant time as N is million

#### Task 3 - Amortized Analysis
Question: Why appending to a dynamic array is amortized O(1), not O(n) even though resizing sometimes costs O(n)
Answer: When the size is lesser, the creating new memory location will happen frequency as data is increasing, but when we are in larger scale, the reallocation happens rarely. that's the reason we call it as O(1).
Note: this is not correct answer as I know, need to get real answer from chatGPT

#### Task 4 - Precision Check
Answer Yes / No
1. Is O(2n) different from O(N)?
   No. as constant we can ignore when it's Big O, as it won't make differences
2. Is O(log n) always faster than O(n)