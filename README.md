# UA workshop - Higher/Lower game

The goal of the workshop is to create a higher/lower game. The player will see a number between 0 and 10 and has to guess if the next number will be higher or lower.

1. Create a <Game /> component. It should should show the current number, give the player the 'Higher' and 'Lower' choices and display the current score. If the game is finished (after guessing incorrectly) the player should see a request to submit his/her score and a retry button. Provide an 'onSubmit' event prop with the player name and score as params.
2. Add the <Game /> component to <App />. Use the info coming from the 'onSubmit' event to display the name and score of the last game that was played.
3. Create a <LeaderBoard /> component. It should show a table of players names and scores sorted from high to low.
4. Add <LeaderBoard /> to <App /> and create some state in <App /> to hold all the highscores (not just the last one). This state should flow down to <LeaderBoard />.
5. Create a <Tabs /> component. It should display titles of the tabs and only show the content of the active tab underneath.
6. Implement the <Tabs /> component in <App /> and put <Game /> and <LeaderBoard /> in separate tabs.
7. Create ScoresContext, <ScoresContextProvider /> and useScoresContext. The context should hold all the highscores and a function to add a new score (all exposed through the hook). Add the <ScoresContextProvider /> to the 'main.tsx' file.
8. Use the useScoresContext hook in <Game /> to replace the 'onSubmit' event.
9. Use the useScoresContext hook in <LeaderBoard /> to display all the scores. This will replace the current prop.

### Extra

10. Persist the scores in localStorage so they do not disappear after refresh.
