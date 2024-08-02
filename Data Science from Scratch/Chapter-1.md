# Introduction to Data
Everywhere you look, there's more information than ever before. Websites track what you do online, your phone knows where you are, and even special fitness trackers keep tabs on your health. All this stuff is basically a giant mountain of information, that if used correctly can reveal hidden secrets in our daily lives and even change them for the better.

A data scientist is a professional who can extract meaningful insights from all kinds of data. Data scientists also have some basic knowledge of programming and statistics and other fields of mathematics as well.

People then use these insights to track habits and figure out where are they lacking and where can they improve. Companies use these insights to provide better customer experiences and products by targeting the customers based on their previous search and purchase history.

## Everything is connected
Everything is connected to everything in some way, shape, or form.  For example, in order to find the "key connectors" in a database of a social media website in order to make the suggested persons to follow or connect with better.

We can examine the ids of the user and the ids of the users that they are friends with. Then we can examine if any two people are connected to a third person but aren't connected to each other.

``` mermaid
flowchart LR
 A(Person one) --> B(Person two)
 B -- Maybe knows --> C(Person three)
 A --> C
```

Different people can be friends of friends and not know each other. The more users the website has the more difficult this process will be.

Counting the number of friends of a person and then making connection between them based on their mutual friends to suggest them people to follow and connect with is a somewhat better approach to this.

This approach can be applied for people that are in same groups or have the same interests as well. We can also create a system where we pick a common  interest among users that may or may not be friends and suggest them new people based on the common interest.