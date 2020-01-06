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

- [https://www.atlassian.com/blog/archives/git-guilt-blame-code-review](https://www.atlassian.com/blog/archives/git-guilt-blame-code-review)
	- code review is an amazing tool to increase code quality
	- higher chance of finding bugs and reduce technical debt before product delivery
	- spread information and knowledge around the team
	- responsibility for the code is spread to more than one person
- [https://www.atlassian.com/blog/archives/creating_optimal_reviews](https://www.atlassian.com/blog/archives/creating_optimal_reviews)
	-	do not overload the code review (e.g. too many files)
	-	do not review with too many reviewers

## [JetBrains Best Practices](https://blog.jetbrains.com/upsource/2018/08/30/code-review-best-practices/)
1. The reviewer should not concern about whether the code compiles or not, so provide an automated CI-pipeline to guarantee compiling and tested code.
2. As a team you should agree on code review goals before and checking the definied aspects explicitly on each review.
3. Create merge requests linked to a branch (and so to a specific ticket) if useful.
4. Labeling comments is helpful for quick understanding the intention (e.g. Bug, Code Style, Security issue, Explanation, Design, Other).
5. As a reviewer, you should also leave positive feedback in code reviews.
6. Code reviews should be iterative. That way, reviewers have to read less code at once and are part of the process.
7. Discussions in code reviews should be marked as resolved when there is no more action needed.
8. As a team, agree on criteria for closing a review. It can be necessary that all assignees need to approve or just a subset.

## [Code Review Best Practices](https://youtu.be/hVJGu0xdXII)
1.	Aim of code reviews
-	it is an addition to static code analysis due to the aspects, software like sonarqube has its limitations (it cannot evaluate readability or naming of variables, methods etc.)
-	it adds value to your system in view of maintainability (e.g. readability), operations (e.g. proper exception handling), scalability and performance
-	it adds value to your team / people by sharing knowledge and gaining new experiences among each other
-	it adds value to your team by identifying best practices and common patterns / mistakes
2.	When to do code reviews
-	as early as possible
-	during the sprint
-	new changes (developer joined or technology / method changed) -> more detailed review
3.	How to do code reviews
-	pair programming reviews
-	sometimes fixing something directly can safe time instead of writing a comment
-	static code analysis tools (e.g. sonar) can help
-	JUnit tests can be an indicator of the complexity of code (easy tests -> easy code)
4.	What do you look for in code reviews
-	architecture
	-	communication
	-	chosen frameworks
	-	testability and reuseability of the components
-	design
	-	interaction between classes
	-	unit tests
	-	programming principles (e.g. SOLID)
-	code
	-	formatting
	-	complexity
	-	readability
-	performance
	-	caching
	-	session usage
	-	object creation
-	language specifics



Notes:
-[https://www.deepcode.ai/](https://www.deepcode.ai/)
<!--stackedit_data:
eyJoaXN0b3J5IjpbMzU2Njg5MDc1LC01Mzc5MTU4OTksMTQ2MD
EzMzk2MCwtNDY5NTQwNDQ2LDE3MDQ1MjQxMjgsLTIwMzU0MDU4
ODIsOTE1MTY1MzI3LDE5MjkzMDEwNTEsMjM3NDc1MTYwLC0xND
Q5OTcxMzEwLDE3NTA3MDIyOTIsMTAxODExMzg2MSwxMzg1Mzk2
NzM0LDE3NjY3ODMzOTIsMTg5MTY2NzEzMSwtOTg1NDMxMDY1LD
ExMjk2NDU1ODEsMTkwNzM3OTk2MSwtMTUwMjkzMjNdfQ==
-->