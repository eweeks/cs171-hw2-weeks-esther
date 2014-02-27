Esther Weeks Problem 3 - Homework 2 (Plus design paragraph)

1. I think the ideal Network Graph would need to address or have the option to address 
a variety of tasks. As the networks and how they are used varies a lot on GitHub,
the most successful graph would allow for some flexibility in layout that the user can 
specify. Having said that, for all users, the Network Graphs primary role is to give
an overview of that repository. 
	Important task, that help create this overview are as follows:
	1. Show Connections
		For a successful Network Graph, this should include several types of connections,
		and includes:
			-Connections between commits and users. 
			-Connections between branches
			-Connections between users and branches
		
	2. See Activity
		Once again, there are several activity categories to look at. 
			- User activity
			- Activity on a branch
			- Commit activity  
			
	From the reading for this question  (Lee et al., 2006). I would say the graph-related
	tasks would be sort and scan. I feel sort and scan apply both to seeing connections 
	and seeing activity. For example a successful network graph would allow the viewer
	to sort the branches (either physically on the screen or visually), and then 
	scan that branch for user activity. I feel in this graph the sort and scan complement
	each other. Based on the reading, it could be said the graph task taxonomy could be
	Adjacency and Connectivity. From the description, connectivity includes finding the 
	most direct connections, identifying groups and identifying connected components, all 
	of which are important in this graph. Adjacency is described as finding nodes which 
	are next to one another. I feel Connectivity better fits the role of this graph, 
	though either could apply. 
	
	2. Having looked at these repositories and others through the course of this assignment
	it seems there is variation in both the interaction between branches and the 
	interaction between users. On some repositories the majority of the interaction
	between the branches occurs towards the ends of a branch, either shortly after
	that branch was created, or as seems more common, when that branch is merged
	back into the master. Larger repositories, including the D3, jQuery and BootStrap, 
	have more and more frequent interaction between branches. The interaction between
	the users also varies, and probably has to do with work methods and collaboration 
	methods on that repository. On some repositories, users work on one or just a few 
	branches at a time, while other repositories have users making commits to a large
	number of repositories. In BootStrap for example, most of its users are only active
	on a few branches at a time, but there a couple of collaborators who seem to be
	involved on all the branches that are currently active. D3 is similar, but on a 
	smaller scale, where most of the users are only working on one branch, but one
	user (Mike Bostock) is involved on them all.
	
	
	3. Larger data sets get cluttered very easily, and it becomes harder to see the 
	connections. It's also much more difficult to view it all on the screen, so it 
	looses the ability to allow a user to quickly scan all the data. With more
	frequent interactions between users and branches, it changes some of the spacing
	of the data, and can create more overlap between nodes and links. 
	
	The varying connections, and varying work patterns mean that some amount of user 
	control on how the data is shown would be valuable. I initially had been coloring
	my data and sorting by branch, but realized this was not what was shown in the
	problem set, so I added an option to sort by author or by branch. After looking at
	the 3 listed repositories and multiple others to see the trends, I can see how
	sorting options like this are very valuable. 
	
	
	4. Keeping the initial graph view simpler at the start, and giving the viewer more 
	information on exploration, would help keep the graph cleaner and I think would
	work better both for small and large data sets. Adding to this, would be adding more
	sorting options, this will allow the viewer to adjust the data to better see the 
	connections they are most interested in. Sorting options could include:
	 author:
	 	Could sort by most active, least active, or alphabetical
	 branch:
	  	Could sort by time, most recent, oldest
	 Both author and branch could also be sorted by most active and least active.
	 
	 In helping to keep the graph cleaner and less cluttered with larger data sets,
	 a branches commits could be shown only on hover. This way if a viewer was interested
	 in viewing more detail on a particular branch they still could do so easily, but it 
	 would clean up the view otherwise. 
	 
	 I feel it may also be beneficial to adjust the layout of the graph to better fit the
	 screen. This could allow for more of the data to be viewed at once and thus give a
	 better overview of trends. 
	 
	Other items come to mind, such as showing the amount of activity on a branch
	at a glance, perhaps by making the lines thicker if there are more commits.  It also
	would be nice if the categories (author, or branch name) would stay stationary, while
	the graph can still scroll. This way if you are looking at data at the bottom/end of 
	the chart you can still see the category names. 
	
	Design Sketch Paragraph:
		In addressing the problem of clutter with larger data sets, my design has a vertical
		orientation instead of a horizontial one. This is easier to scroll through for
		a viewer and allows more of the data to be shown at one time. Ideally
		the view will expand to fit the data set. Also to eliminate some of the clutter
        in the graph, nodes or commits will only show up when the viewer hovers over the
        branch.
        My design focuses on the big picture first and then has more details and information
        available upon exploration. I wanted to show the connections while still maintaining
        readability. Color and lines will be used to represent the connections themselves.
        Lines will show the branches, and vary in weight based on how many commits are
        made on each branch. It might by possible to create an effect similar to a Sankey 
        diagram by doing this. Other lines will show the connections to other branches. These
        will be differentiated from the branch lines by weight. Shapes will be used to show
        the commits themselves, either circles or squares. 
        Ideally, my design would have multiple sorting features, allowing the viewer to see
        the data in multiple views and thus adjust to the varying users and their different
        work methods on GitHub. 