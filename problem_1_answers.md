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

Make a call to that users info, get a list of all there commits for that year, opened issues,
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

