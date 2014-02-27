Esther Weeks Problem 4 - Homework 2

The technical and design choices on this project fall into a few categories:
1. Layout, 2. Lines, 3. Color, 4. Sorting Features, 5. Issues/Skill and Time 
limitations.

Layout: I was successful in creating the basic layout I was hoping for. My chart does
go vertically, and I was also able to have a header which did not scroll, allowing for
a clearer view of the heading categories for the whole length of the chart. I was also
able to set the height of the chart to adjust with the dataset. I did this by taking
the number of commits in the data and multiplying by a padding number to give some space
between each node. This seems to work well, and was tested on multiple datasets. As 
previously mentioned, I was thinking of keeping the layout rather simple, and I did
stick with this. I did consider trying to create a layout similar to a Sankey Diagram, but
I did not feel I had enough time to try and implement this and was also concerned with
it being easily scaleable for different data sets.

Color: I used color to help show the connections on the GitHub graph. Different colors
relate to different branches. I also used color to show where the focus is. On hover,
the color of the nodes is lighter than that of the bars and the node being hovered is
red. Color helps to make the chart more readable and easier to scan for information.

Lines: Lines are also used to help show connections. In the authors view, the branch lines
and nodes are larger based on the number of commits a user has made. This helps the viewer
to see where the activity on the repository is. In both the author and branch view I chose
to make the lines representing the links between branches or users, thinner and dotted.
This created a visual difference between the tow, making the chart easier to process.

Sorting: Sort may be done by author or branch. Ideally, I would have implement more sorting
options, for example, allowing to sort by user either ascending alphabetical or descending. 
The same could be applied to branch name. It would also be helpful to sort by amount of 
activity, showing the most active branches to least active for example. I would also
like to have options that would allow for showing more information about the repository.
Showing the currently open issues, for example, and which branch they are one. Also
showing amount of activity in a commit, such as additions and deletions. 

Issues/Skills and Time limitations:
	My biggest issue was working with the GitHub data to understand what was going on, 
	and thus be able to understand if I was correctly representing the data, but also 
	therefore knowing if the code I wrote was correct and working how I invisioned. 