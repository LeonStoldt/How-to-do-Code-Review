# Code Review - Best Practices

## [Atlassian Summit 2016](https://www.youtube.com/watch?v=fatTnX8_ZRk&t=5s)
1.	Restrict the scope of a merge request to one issue (implies well-designed issues in view of size).
2.	Mapping between features and branches makes the workflow easier (new changes to the issue cause new changes to the branch and so to the merge request).
3.	Mirror the process / workflow to Jira (or other issue tracking systems) to implement the review process to the workflow.
4.	Let the merge request be approved by at least two other developers.
5.	Assign the merge request to a minimum of three developers to avoid waiting times for cases like someone is overloaded or sick
6.	Do not assign to many reviewers in light of the fact too many will reduce the number of errors found. In addition, it will lower the invested time, the more reviewers are assigned.
7.	Pick your reviewers by taking a look at git-blame in order to assign it to the author. If you are having problems to find other candidates, take a look at git-guilt as well to see who else was involved over time.
8.	`@mention` reviewers to specific parts of code where they are experts of.
9.	In order to avoid issues getting stuck in review process / lane, define an explicit day of the week for finishing off all merge requests left.
10. Questions and discussions coming up in the merge request should considered to transferred to the code as a comment to avoid the same questions of future developers.
11. For code changes involving UI / UX changes, add screenshots / gifs / videos [with Monosnap, GIPHY, ScreenFlow] to your merge request to simplify understanding for the reviewers. (now you can assign non-technical stakeholders as well to)
Even better than screenshots is a separate instance where the changes are deployed.
12. The more lines of code a merge request has, the less amount of time will be spend by the reviewer. So keep the reviews as small as possible and push changes incrementally.

## [JetBrains Best Practices](https://youtu.be/EjwD7Pi7J_0)
1. The reviewer should not concern about whether the code compiles or not, so provide an automated CI-pipeline to guarantee compiling and tested code.
2. As a team you should agree on code review goals before and checking the definied aspects explicitly on each review.
3. Create merge requests linked to a branch (and so to a specific ticket) if useful.
4. Labeling comments is helpful for quick understanding the intention (e.g. Bug, Code Style, Security issue, Explanation, Design, Other).
5. As a reviewer, you should also leave positive feedback in code reviews.
6. Code reviews should be iterative.
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTQ5ODc4NjE0MiwxODkxNjY3MTMxLC05OD
U0MzEwNjUsMTEyOTY0NTU4MSwxOTA3Mzc5OTYxLC0xNTAyOTMy
M119
-->