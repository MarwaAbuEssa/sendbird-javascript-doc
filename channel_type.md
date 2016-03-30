# Channel Type

There are some terms you should understand before starting this tutorial.

###**Open Chat**

Open chat is a public chat. This is a channel type which anyone can participate without a permission. It can handle thousands of users in one channel. ex) **Twitch-style public chat**

###**Messaging** 

Messaging is a private chat. The user who wants to join the messaging channel has to be invited by other user who is already joined the Messaging channel. 
  * **1-on-1 messaging** : 1-on-1 messaging is a private channel between two users. The same channel is always reused. If a new member gets invited to the 1-on-1 channel, then a new Group messaging channel is created and the original 1-on-1 channel remains the same. ex) **Twitter-style Direct Message**
 
  * **Group messaging**  : Group messaging is a private channel among multiple users. You can invite upto hundreds of members into the Group messaging channel. ex) **Whatsapp-style closed group chat**

||Open Chat|Messaging|
| -- | -- | -- |
| Access Control | Public | Invitation required |
| Class Name | Channel | MessagingChannel |
| Number of Members | Over a few thousands | Less than a few hundreds |
| How to create | SendBird Dashboard / Server API | Client SDK / Server API|
| Moderation | User Mute | User Block |
| Unread counts | N/A | Supported |
| Read receipts | N/A | Supported |
| Typing indicators | N/A | Supported |


