# CS-353-Project-Reports
# 

**CS 353 Project Proposal**

**Social Media for Hosting Events - Find&#39;N Meet**

**Berk Ataç - 21200623 - Section 2**

**Kaan Tapucu - 21402172 - Section 2**

**Melih Ünsal - 21501085 - Section 2**

**Engin Deniz - 21301826 - Section 2**



# 1.Project Description

In this project, we are planning to design a system for people to host events for anybody having similar interests. We are going to have people, events, categories, cities, groups and messages entities so that we can come up with an entity-relation diagram for the system. Users of the system will be able to create a specific event according to their interests. Then, they can send invitations to their selected friends along with making the event public if desired. Events are specific to a particular location and time. It means that when an event is created, it will have start and end time as well as address information where it takes place.  Additionally, for each event, there is going to be quota for the event so that we can put a limit on participants so as not to encounter with any problem related to availability of the place. People who joined the event will be able to be reviewed by event hosters. Users will be able to create a group. Moreover, they will be able to share their comments to a group&#39;s forum as well as an event&#39;s forum. However, in order to make a comment to an event, they should participate to the event. For this project, we are going to use a database where all of the information of these entities are maintained. The reason why we are planning to use a database is that users will be using our system concurrently. It means that using a database rather than file system is rational. Most importantly, we need to prevent data redundancy and inconsistency by making use of creating a database system.

# 2.Funtional and Non-Funtional Requirements

2.1Functional Requirements

**Sign Up:** People who want to become a member will sign up by creating a username and password. Also they will share additional info about themselves. Full name ,age, gender, address, profile picture, job and a brief description about themselves. During sign up process they will create their profile.

**Log In:** If already a member, user will need to enter their username and password and log in.

**Join Event:** Users will circle through events according to their choice of category, address and will be able join or request to join an event based on the privacy setting on an event and its remaining quota.

**Create Event:** Users will be able create events for other users to join. They will enter event&#39;s name, address, time slot, quota, description, a picture and privacy setting. Privacy setting can either be public or private. Any user can see and join or request to join public events. Not all users will be able to see private events. User will need to get an invite for seeing and joining private events.

**Create Group:** Users will be able to form groups with other users with similar interests and their friends. Forming a group will require entering groups name, category, description and a picture. Other users can get an invite or send a request to join in groups.

**Join Group:** Users will be able join a group with interests similar to theirs by getting an invite or by sending a request to join. Group admin will either send invites or accept requests in order for users to join.

**Send Message:** Users will be able to communicate with each other by sending messages. User will select another user and send them a message which only sender and recipient can see.

**Comment:** Users will be able to address to more than one user with comments. They will either comment on event pages or group pages in order to ask questions, share their opinion or general communication.

**Choosing a Category:** Users will click on the category option in order to search for an event or a group under that category.

2.2 Non-Functional Requirements

1)          Page, button and background designs will be appealing and dynamic.

2)          No private information will shared with public.

3)          Internet connection will be required.

4)          Software can be accessed on any device with internet connection. IOS, Android, desktop etc.

5)          In order to use the software, users must be older than 15.

** **

#  3. E/R Diagram


![](https://github.com/Seftali/CS-353-Project-Reports/blob/master/ERdiagram.jpg)


messaged(sender\_ID, receiver\_ID, context)

create\_group(group\_ID,people\_ID)

joinToGroup(group\_ID,people\_ID)

send\_comment(comment\_ID, people\_ID)

joinToEvent(event\_ID,people\_ID)

create\_event(event\_ID,people\_ID)

lives(people\_ID, address\_ID)

take\_place(event\_ID, address\_ID)

when(event\_ID, time\_slot)

event\_belong(event\_ID, category\_ID)

group\_belong(group\_ID, category\_ID)

group\_event(event\_ID, group\_ID)

event\_has(event\_ID, comment\_ID)

group\_has(group\_ID, comment\_ID)

# 4.Resources

[https://www.draw.io/](https://www.draw.io/)

[https://www.meetup.com](https://www.meetup.com)
