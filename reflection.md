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
  - I used Claude Code.
- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result).
  - The AI suggested swapping the hints for higher/lower so that they showed correctly and it fixed the bug successfully.
- Give one example of an AI suggestion that was incorrect or misleading (including what the AI suggested and how you verified the result).
  - When creating the tests for my bug fix, running pytest did not work. The AI suggested creating the conftest.py file. It explained to me that, "Adding an empty conftest.py at the root tells pytest to treat the root as the base directory and adds it to the path automatically."

---

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed?
  - I tested the game myself by trying the game out and seeing if the new code met my expectations.
- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code.
  - A manual test I ran was testing to see if the "New Game" button reset the attempts (to start at 1), score, status, and history. 
- Did AI help you design or understand any tests? How?
  - Yes, it helped me design tests to assert that the different difficulty level ranges were accurately set. I asked the AI to write a test to target the function of accurately changing the ranges based on the level of difficulty selected by the player. Easy should be 1-20, Normal 1-100, Hard 1-200.

---

## 4. What did you learn about Streamlit and state?

- In your own words, explain why the secret number kept changing in the original app.
 - It changed whenever a new game was started. Didn't notice any weird behaviour otherwise.
- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?
  - Streamlit runs the app, then you must refresh the page in order to reset the app.
- What change did you make that finally gave the game a stable secret number?
  - The new game button was fixed.
---

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
  - This could be a testing habit, a prompting strategy, or a way you used Git.
   - Giving my expected results and what the bug currently does and how that is not what I need.
- What is one thing you would do differently next time you work with AI on a coding task?
  - I would ask it for more explanation on things I do not fully understand so that I don't have to go back to it later.
- In one or two sentences, describe how this project changed the way you think about AI generated code.
  - The more context the AI is given, the better results it will produce.
