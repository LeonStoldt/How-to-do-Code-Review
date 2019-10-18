# Code Review - Best Practises

## [Atlassian Summit 2016](https://www.youtube.com/watch?v=fatTnX8_ZRk&t=5s)
1.	Restrict the scope of a merge request to one issue (implies well-designed issues in view of size)
2.	Mapping between features and branches makes the workflow easier (new changes to the issue cause new changes to the branch and so to the merge request)
3.	Mirror the process / workflow to Jira (or other issue tracking systems) to implement the review process to the workflow
4.	Let the merge request be approved by at least two other developers
5.	Assign the merge request to a minimum of three developers to avoid waiting times for cases like someone is overloaded or sick
6.	Do not assign to many reviewers in light of the fact too many will reduce the number of errors found. In addition, it will lower the invested time, the more reviewers are assigned.
7.	Pick your reviewers by taking a look at git-blame in order to assign it to the author. If you are having problems to find other candidates, take a look at git-guilt as well to see who else was involved over time.
8.	`@mention` reviewers to specific parts of code where they are experts of.
9.	In order to avoid issues getting stuck in review process / lane, define an explicit day of the week for finishing off all merge requests left.
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTE3MzQzMzUwMiwtMTUwMjkzMjNdfQ==
-->