# ViiMe
<img src="ViiMe-Transparent.png" style="height:150px">

ViiMe was a project created by my best friend and one of his friends. The idea was that venue owners could provide unique deals to people if they come in groups. The project required creating a web application for venue owners and a mobile application for patrons. 

There major requirement was that the application must be available on both iOS and Android

## Mobile

### Background
The mobile application was the method for patrons to easily redeem deals at specific venues. They would need to search through venues, find a deal they like, and then be able to redeem it. 

When the user first opens the application, they will land on the Login page. They must enter a username and password to login. If they do not have an account, they can click a 'Not a member? Sign up now!' button. If they forgot their password, they can click the 'Forgot Password?' button.

<img src="Login .jpg" style="height:350px">
<img src="Sign Up.jpg" style="height:350px">
<img src="Forgot Password.jpg" style="height:350px">

After they login, they will head to the groups page. To redeem deals, users must form groups by inviting their friends. If there are any active groups to redeem deals, this is where they will appear. The reason for having groups is that we can track who has redeemed what deal, and this information can be conveyed to venue owners. They can redeem any deals or invite friends to deals on this page. When they want to redeem, a pop-up appears where a code must be entered. Employees at venues know this code, and would enter it in for the deal to be redeemed.

<img src="GroupsPage.jpg" style="height:350px">
<img src="InviteFriend.jpg" style="height:350px">
<img src="GroupsInvitations.jpg" style="height:350px">

From this page, there are 3 places to go: the profile page, friends list page, or to browsing venues.

The profile page is where users can update their personal information. Another feature the founders wanted was 'vRewards'. 
There were rewards sent directly from venue owners to users to thank them for their loyalty.  

<img src="Profile.jpg"  style="height:350px">
          
The friends list page lists all friends, and there is a button to add a friend. When adding a friend, they will type in the username of their friend and all possible matches will show up in their search.

Finally, they can browse venues. On this page, all venues with deals are listed. They can search through the venues and when they click on one, they will see venue information and deals. If they click on a deal, they will see the possible things they can redeem depending on how big their group is. On the top right, there is a button to invite friends to their group.

<img src="VenuesOriginal.jpg"  style="height:350px">
<img src="VenuesDeals.jpg"  style="height:350px">
<img src="Deals.jpg"  style="height:350px">

To summarize, the current application flow is shown below.

<img src="Navigation1.png"> 

The next step will be to improve the interface through this course. We will start afresh with user requirements.

####  User Requirements

With the application published, feedback was collected from users. Furthermore, I asked 3 friends with no prior knowledge of the application some questions. I wanted to see how they would navigate the application and where some chokepoints for users might be, along with their general impressions of the application.

I asked three simple questions which I thought would give some key insights. They are as follows:

1. Please redeem a deal (the deal to redeem was given)
2. What are your overall impressions of the application?
3. What would you improve?

To summarize findings, here are the key points:

- Users really did not understand the concept of having to create a group, invite your friends (which means adding friends to your friends list), and then redeeming.
-  There were some layout concerns, especially with the venue information page and deals page.
- They liked the idea of the application, and the deals offered
- They did not understand what vRewards were


The major point of concern is not understanding the concept of a group and why that was necessary. From a business stand point, the founders really wanted to be able to track exactly who was redeeming what deals. They wanted to use this information and sell it to business owners. This was something I pushed to them earlier that this whole process of creating groups would be a big headache for users (and to implement). After conducting these interviews, I brought it up with them again and pushed them on it. They finally gave in - get rid of this groups concept.

The reason why it makes sense to get rid of creating groups and redemptions is that, instead of doing that, users should just be able to log in, look at a venue, and bring up the redemption page. The employee at the venue can look at the # of people in the group and then punch in the redemption code. This makes it significantly easier to redeem a deal you want.

####  Navigation

With this new information structure, the whole navigation was re-thought. It was not necessary to have groups to redeem deals. Thus, the concept of friends list was not necessary. Furthermore, the whole navigation layout was simplified:

<img src="InformationStructure.png"> 

####  Layout

This change required changing some of the page layout. Instead of having a deals page where as they invite more users, the deals change, it makes more sense to list all the deals. This way, when they click a venue, they can see all deals, how many people they need, and they can decide which deals they want to redeem. After clicking the deal, a popup will show where employees can enter a redemption code. Another quick idea was to change the venue layout. Since rows for each venue were taking up a lot of space, and there are currently ~15 venues in the application, it takes up too much screen space. A quick sketch of these new layouts are shown below:

<img src="Layout.jpg">



The venues are now 'cards' and two cards can go in one row. Furthermore, the deals will be listed when they click the venue, and right after clicking the deal, a pop-up shows up where they can pass the phone over to a venue employee to enter the code.



