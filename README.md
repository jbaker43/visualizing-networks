## Dataset 1: Car Sales

## Description

### Dataset Format: Tabular

The first dataset that I wanted to try and visualize was a .csv file containing every
automotive manufacture’s sales figures. It contains a lot on interesting information that would
be great to visualize in other assignments. There are different columns of data including resale
price, engine size, horsepower and so on. For this visualization I mainly focused on using the
columns of ‘sales in thousands’, and ‘price’. Since the file that was provided is .csv. This could
be considered a tabular dataset. However, I am representing the data in a hierarchical tree
map. With each model of car having the parent being the manufacturer, and the parent to the
manufacture being the auto industry in its totality. Representing the data this way allows up to
see how each model of car plays a role in overall sales for not just a company but in the entire
automotive market.

### Data Type: Items

This dataset is made up of item-based data point as each unique row represents a
unique model of a brand with its corresponding data points such as price, weight, first on sale,
horsepower, etc.

### Attribute Types and Semantics

This dataset contains attributes that are both categorical and quantitative. Overall there
are 158 rows containing 16 quantitative and qualitative data points. ‘Manufacture’, ‘Model’,
and ‘Vehicle type’ are categorical or qualitative attributes. Without assigning a quantitative
value to these attributes, you cannot assign a scale to them, they are categories. The rest of the
data columns are all quantitative. It is easy to assign a meaningful scale to them. You can easily
say that the BMW 32 8 i is a more expensive car than the BMW 323 i by about 9 thousand dollars.
The semantics of the dataset are clear. The dataset allows us to easily visualize a myriad of
different things apart from a hierarchal tree map. Using this dataset would allow you to easily
pit different brands against each other or even different models within a brand to draw some
conclusions. For example, we could look at what is the most fuel-efficient brand overall by
averaging all the MPGs from each brand.

### Preprocessing

Originally, I removed all ‘nan’ from the dataframe but that in turn removed all of Volvo’s
entries and all od BMW’s entries. I removed this line of code and left it as is, so no
preprocessing was needed.


### Visualization

As stated above, I wanted to see the hierarchal structure relationship that each model
of car plays in each brand. That would allow us to see overall sales in the market grouped by
manufacture and model.
![](https://i.imgur.com/sHfW5I8.png)

### Analysis

Straight away I was surprised at just how many Ford F-150s are sold. Apparently, this is
nothing new for Ford as they sold over 85 0,000 F-150s in 20 20. Another thing that I noticed
right away is that the Chevy Silverado is not on this list. That leads me to believe that this list
predates the launch of that truck which was in 199 9. Looking at some of the other models from
other manufacturers would confirm this. For both Ford and Dodge, pickup trucks are their
number one selling model by almost double in both cases. Furthermore, somethings do not
change as the Toyota Camry was their number one car then and still is! I think it is easy to
overlook just how many F- 150 s are on the road. After looking a little further, I was able to find
that Ford has sold over 26 million F-150s. That’s enough to give every single person in Australia
one and still have 300 thousand left over.


## Dataset 2: My LinkedIn Connection Network

## Description

### Dataset Format: Tabular

For my second dataset I was struggling to find network type datasets to visualize. I was
able to download my data from LinkedIn and visualize my connection though the use of pyvis as
a network. After requesting my data from LinkedIn, they send you a link to download the file. It
was provided to me as a .csv file. Thus, it’s in the tabular format, however we will be
manipulating it to use as a network dataset.

### Data Type: Items

As stated, the dataset was downloaded as a .csv containing item-based data types with
each column corresponding to a connection I have made on LinkedIn.

### Attribute Types and Semantics

This dataset contains all categorical data except for one column that is a quantitative
data point which is the data I connected with that person. We could easily assign a scale to this
column and figure out things such as how many days has it been since I made a connection, or
on average how many connections do I make per week, and so on. The rest are all quantitative.
They are first and last names of my connections, emails if they chose to show that on their
profile, and their organization, as well as their position at their company or organization. I do
not have many connections on LinkedIn, so the total size of this dataset is only 41. However,
since we are grouping people into their respective companies, the size shrinks down to 29.

### Preprocessing

This dataset required a little bit of preprocessing. The first is that I needed to read in my
downloaded file as a dataframe but skip the first two rows as LinkedIn adds some information
at the top we won’t be needing. After that I created a new dataframe that takes a count of each
company and sums its. The new dataframe is just the company and the corresponding count.
From there we could

### Visualization

I was able to complete the visualization of my network using pyvis. I set me at the center
of the network and had each node represent a different company my connections work at. The
nodes were either bigger or smaller depending on the number of connections I have there. I am
not the biggest user of LinkedIn by any means so this is a little underwhelming, but I believe the


principal remains that this could be a really interesting visualization for people with a lot of
connections.
![](https://i.imgur.com/QoRvlwA.png)

### Analysis

I wish I had more connections because it would be easier to see more trends and
patterns for this network. However, I was able to see that the people I connect with the most is
at The University and at TVA. These both are not any surprise to me as people I connect with
here at the university are my peers and people, I connect with at TVA are my peers that have
since moved on to their career there. It was interesting to see all the different company names
and try and remember why they are connected with me. I must admit there were a few that I
had to go and look up! Overall, I found this to be an interesting way to try and visualize a
network with different nodes and edges.
