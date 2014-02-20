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

Commits:

Who is the audience?

The audience is collaborators on a specific project, probably once again geared towards
the project manager, although there might be situations when it could be helpful for other
members of a project to view. This shows a yearly overview of the project commits, keeping
track of which weeks had the most commits, and also divides this down further into days. 
As this doesn't show specific data for any contributors, but general information for the
project, it is probably most relevant for those either managing the project or those 
very involved in the current year. 

What data is used?

The data comes from that specific repository. It is the number of commits and the dates of
these with in the current year. It is keeping track both of the number of commits per week,
but also the number of commits each day. 

How can you get the data using the GitHub API?

Make a call to that repositories info, get a list of commits, with dates included for the
current year.
  //api.github.com/repos/username/repository_name ... then somehow narrow 
this down...  //api.github.com/repos/username/repository_name/commits will give list of 
commits... also has the dates

What happens if suddenly a contributor pushes many commits in a short time interval? 
How would you address this particular issue? 

This graph doesn't have a way of keeping track of contributors. If a contributor pushed
many commits in a short time, it would create a spike for that day and probably that week
in the visuals, but would not show who made those. If viewing this information was important
you could create a tooltip that would show up when you hover over either the bar or the circles
on bottom graph. This could give you more of a break down of when these commits were made and
by whom. 

Code Frequency:

Who is the audience?

Code frequency doesn't keep track of contributors either, so I feel this also would be primarily 
useful by project managers and those closely involved with the project in the past year. 
This graph gives an overview of additions and deletions on this project, and would be of 
value to anyone interested in the yearly changes for that specific project. 

What data is used?

The data for this is similar to the data used in the commits graph. It also is specific to
the repository, using the dates of the commits in the past year, but this time also using
the number of number of lines added and deleted in each commit.

How can you get the data using the GitHub API?

Make a call to that repositories info, get a list of commits, with dates included for the
current year.
  //api.github.com/repos/username/repository_name ... then somehow narrow 
this down...  //api.github.com/repos/username/repository_name/commits will give list of 
commits... also has the dates..don't see anything on additions or deletions though...

What happens if suddenly a contributor pushes many commits in a short time interval? 
How would you address this particular issue? 

It would probably show as a spike on the graph, either a spike of additions or deletions, 
unless there is a lot of general activity on that repository, then as the scale is set
to show the trends through out the year, it would probably be lost in the curve of the 
data. As this graph aslo doesn't show the contributors who made these commits, it
doesn't really address this. If you wanted to show the contributors who added the 
data, you could add a click function that would allow for clicking on the graph and 
getting more detail of who made those changes in the selected area. 

Punch Card:

Who is the audience?
Punch card shows general data for the whole repository, with nothing specific to the 
contributors. Once again, I believe it is most useful for the project managers though also
with situations when it would be of interest to other contributors on the project. This is a 
useful graph for those who are interested it what time and days most of the work was done, 
as it graphs the commits based on day and time. This could be useful in situations where 
you are either looking for a time when the most people are working or a time when they probably
will not be. 

What data is used?

This graph uses commit data from the specific repository, it seems, across the entire history of
the repository, not just a year. It is using both a count of commits as well as a day and hour
associated with each. 
  
How can you get the data using the GitHub API?

Make a call to that repositories info, get a list of commits, with dates for all.
  //api.github.com/repos/username/repository_name ... then somehow narrow 
this down...  //api.github.com/repos/username/repository_name/commits will give list of 
commits... also has the dates..

What happens if suddenly a contributor pushes many commits in a short time interval? 
How would you address this particular issue? 

If it is enough commits, it might show up in relation to the size of the "punch" on the
graph, and the date and time will be recorded and affect the graph. Possibly, this might
make it seem like there is more activity on the repository at a certain time and day, but
if the repository is recording a long enough period, this probably will not skew the data
too much. Once again, if this is something you wanted to show, it could be done by showing
additional data on click or on a hover. 

Pulse:

Who is the audience?

Pulse gives a lot of current information on the project activity and status. I would say it
is very useful for anyone currently working on or managing a repository. It seems especially
geared towards contributors, as it shows new issues, closed issues, pull requests, merge 
requests, number of contributors and number of commits each has made, etc. 

What data is used?

There is a lot of data on this page. This page uses merged and opened pull requests, 
closed and opened issues, contributors and number of commits each has made, number of 
files changes, number of additions and deletions, and unresolved conversations. 
 
 How can you get the data using the GitHub API?
 
 Make a call to that repositories info, get a list of commits, with dates for all.
  //api.github.com/repos/username/repository_name ... then somehow narrow 
this down...  //api.github.com/repos/username/repository_name/commits will give list of 
commits... also has the dates..