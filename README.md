# An exercise in data analysis

This is a small exercise in the kinds of skills that may be required of you.  
The goal here is to evaluate how well you understand the problem, scope it, come up with a strategy to solve it, and execute it.  
More formally, we will look for the following in our evaluation:

## Expected deliverables and evaluation criteria
- Have a working prototype of the task described below. It is fine if your prototype's performance does not match the quality you may have in mind. We value a prototype showcasing all the required tasks moderately well over a prototype which solves just a few of the required tasks very well.
- (We will) assess how well you scope and assess the different components involved which will solve this problem
- Assess how you divide your labor into the components you identify, and how quickly you're able to prototype and finish implementing those components. Remember, there's a time budget of a few days.
- Assess your attention to little details. This is important for us--how much you care for details shows us how much you can own any work assigned to you.
- Assess how you resolve situations when you're stuck.
- Assess how well you communicate and let all stakeholders know of your progress. We emphasize constant communication over receiving no communication for days, and just seeing a dump of the results on the day of your submission. This has multiple drawbacks: (1) it gives us no insight into the process you employ to evaluate a problem and come up with a solution. (2) it gives us no room to help you in case you're stuck on any step. Consider this to be a task you will receive on your job - demonstrate to us how you will work on the task in such a setting.

## Task
The aim is to build a small dashboard which will give us a sense for the kinds of sentiments and discussions happening in a city around a specific topic.
The use-case we will explore is specifically that of a political organization getting a sense for what people are discussing.

## Task 1 - Gather data
Write a function to list out the hot topics that are currently in the news in a city.  
The inputs to this task will be the name of the city.  
Find one relevant source you may want to pull this information from. For example, any one news channel.  
Have a script which displays the top 5 topics currently in the news for a given city.

## Task 2 - Gather relevant discussions
For each of the topics found out in task 1, gather current discussions happening on public forums.  
For the purpose of this task, let Reddit be your information source. You can access free Reddit APIs easily to scrape information from it.  

Note: for each source, there could be multiple discussions that you gather.

## Task 3 - Analyze gathered information
For the discussions that you gather in Task 2, summarize the information being discussed.  
What can you analyze about this information?  
Can you answer the following:
- The main highlights or summary of the overall discussions. This could be a summary across multiple discussions that may have happened.
- What is the sentiment of this discussion? Are people happy, unhappy, dissatisfied, etc.?
- What is it that people are demanding for? What is the actionable needs that people are expressing.

Hint: Use an LLM to gather these insights.

## Task 4 - Build a small front-end to display your analyzed information
Build out a very simple front-end where a user can look at your results and analysis on a webpage.
The webpage should have a form which accepts the city name, and preferably shows drop-downs for each of the sources you selected in Task 1 and 2.  
Given these inputs, show the results from Task 3.

## Instructions to submit your work
- Do not fork this repo. Work on a local copy, and ensure this is a private repository. Add the username `shashank-srikant` as a collaborator, so that Shashank can access the repo as well.
- Make it a habit to push changes upstream to your repo as frequently as feasible.
- Use `Python3.8+` for this work.
- We greatly value reproducability of results. Use `conda` to create an environment and set up your repository. 
- Use a `.gitignore` file to ensure you are not adding junk files to the repo.
- Have a `./src/` folder containing the source.
- Have a `./env/` folder containing the Conda environment file you create for this project.
- Have a `./data/` folder containing all the data your source accesses.
- Have a `./tests/` folder to write out unit tests for key functions. Look up the `unittest` package in Python if you haven't used it before. Also, not every function you write needs to be tested---exercise your judgement and prioritize which function you want tested.
- Keep updating this README with instructions which will help with the reproducability of your work/results.  
- The topmost section of your readme file should be titled `Approach`. In this section, concisely describe the overeall approach you considered to solve this problem. Describe the general strategy you used, the key tools you considered, the different metrics you considered to evaluate your work, and any other detail relevant to the task goals and the evaluation criteria mentioned above.
- Communication: Write an email to shashank@mlexperts.ai with the subject "MLE intern evaluation: \[your full name\]". Shashank will acknowledge your email.
- Please then constantly communicate on the mail thread on how you are approaching the problem, how you are thinking about the solution, progress made, etc. The more updates you share, the more clarity we have on your thought process in solving a problem.
- This task is expected to take **a maximum of 1 week of your time**. It is possible to write this up in two full days over a weekend. If it is taking you longer, please write to shashank@mlexperts.ai explaining your situation.
  
Focus on getting the core functionality right first, and have a working prototype of your solution.  
For any questions, write to shashank@mlexperts.ai  
All the best!
