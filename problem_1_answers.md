Esther Weeks Problem 1 - Homework 2

Calendar Map:

Who is the audience?

The contributor. The data is reflecting all of the contributors public contributions, 
(unless they are looking at their own data, then private contributions are also included)
for one years time. This data, while it may be interesting to a visitor, is probably more
valuable and directed towards the contributor. It gives them an overview of their
activity, allowing them to see quickly when they were most active and least active. The 
graph is also relative to the user. The less/more scale used adjusts with each contributors 
specific trends. What shows up as more active on one persons graph may be less active on 
another, thus personalizing the visual to the specific person, and not showing general 
public trends. 

What data is used?

Contributions over a one year period to public repositories, unless a contributor is 
looking at their own data then the private contributions will show as well. According to
GitHub this includes if the user opened an issue, proposed a pull request or authored a 
commit. Commits need to be created or merged into the default branch of the repository to 
count.  Commits to a fork are not counted, unless they are used in the default branch (not
just in your master branch in your fork). 

How can you get the data using the GitHub API?

Make a call to that users info, get a list of all their commits for that year, opened issues,
and proposed pull requests.  //api.github.com/users/username/events ... then somehow narrow 
this down... 

What happens if suddenly a contributor pushes many commits in a short time interval? 
How would you address this particular issue?

The Calendar Map seems to deal with this well, if you hover over the individual map squares
it will tell you how many commits happened on that day, and if you click on it, below the 
chart it will show you what those commits were to, and a link to see those commits in more
detail. This seems to show a good overview, with more detail available to explore if the 
viewer is interested. Problems with this might be how quickly the data is update to the chart,
and when the personal scale would reset. How many commits would it take to change what is 
marked as more to less, for example. If this suddenly changes, this could present a very 
different graph for a user. Maybe there is some way to alert to user to the change in scale or
reflect the current scale in the view. 

Contributors:

Who is the audience?

Audience seems to be contributors to a certain project, mostly directed to the project
manager. The graph shows all of the commits, additions and deletions made over the life of
that specific repository. It also shows all the contributors and their contributions. This 
gives a good overview of the whole project in terms of when the most activity has occurred
on it, who has contributed the most, and when. As it is not uncommon for contributors to
come and go on project work, based on which pieces they are working on, this is probably 
most valuable for the project manager. It could also be valuable for contributors on the
project to see who else has been working, and maybe get a feel for their own contributions.

What data is used?

The graph is using data from the whole history of a repository, showing the number of
commits, code deletions and code additions. It is showing this data from the master, 
as well as each contributors individual data, including commits, deletions and additions. 
It is also keeping the dates on all this data, and shows on what days what happened. 

How can you get the data using the GitHub API?

Make a call to that repositories info, get a list of commits, deletions and additions for 
the whole history of the project, with dates included. Also need to get which users 
contributed to that repository and keep track of which commits, deletions, etc were
theirs. 
  //api.github.com/repos/username/repository_name ... then somehow narrow 
this down...  //api.github.com/repos/username/repository_name/commits will give list of 
commits... also has the dates and names, 
 //api.github.com/repos/username/repository_name/collaborators will give list
of collaborators, 

What happens if suddenly a contributor pushes many commits in a short time interval? 
How would you address this particular issue? 

This doesn't show up well on this graph, especially on projects that have been around for
a long time, the graphs time will reflect mostly months in these cases, and many commits 
in a short period won't reflect on such a scale, even on the individual graphs. This may
be viewed more clearly with a feature that allowed to zoom in on a smaller period of time,
and possibly also changing the scale to accommodate this. 


