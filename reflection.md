# 💭 Reflection: Game Glitch Investigator

Answer each question in 3 to 5 sentences. Be specific and honest about what actually happened while you worked. This is about your process, not trying to sound perfect.

## 1. What was broken when you started?
1. The hint to go higher or lower seemed to be randomly innaccurate; sometimes it says higher when it should be lower, and vice versa.
2. The new game button does not start a new game as expected. It resets the target but if a previous game was finished, it did not allow for new attempts.
3. The levels of difficulty were wrongly assigned. Normal was numbers 1-100, but hard was 1-50, which does not make sense.
4. Changing the level of difficulty does not actually affect anything. The ranges are still 1-100.
5. Non-numerical numbers can be guessed after clicking submit two or more times. 
6. The history of numbers adds every other number to the history. 

- What did the game look like the first time you ran it?
  - The game looked clean and ready to play.

- List at least two concrete bugs you noticed at the start  
  (for example: "the secret number kept changing" or "the hints were backwards").
  - The total number of attempts displayed on the left hand side did not match the number of attempts that were shown in the middle of the   screen. The left side said 8 attempts while the middle said 7 attempts.
  - The 'higher' and 'lower' hints were always wrong.

---

## 2. How did you use AI as a teammate?

- Which AI tools did you use on this project (for example: ChatGPT, Gemini, Copilot)?
- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result).
- Give one example of an AI suggestion that was incorrect or misleading (including what the AI suggested and how you verified the result).

---

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed?
- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code.
- Did AI help you design or understand any tests? How?

---

## 4. What did you learn about Streamlit and state?

- In your own words, explain why the secret number kept changing in the original app.
- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?
- What change did you make that finally gave the game a stable secret number?

---

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
  - This could be a testing habit, a prompting strategy, or a way you used Git.
- What is one thing you would do differently next time you work with AI on a coding task?
- In one or two sentences, describe how this project changed the way you think about AI generated code.
