# CSCI466-GroupProject
CSCI466 group project 

Application The application you will be designing and implementing will be a web-based, database driven tool to facilitate the running of karaoke events at a bar or other venue. It must allow users to sign up to sing songs from the list of available songs, and also provide the DJ information needed to call up the next singer.

 Searching for songs :
The potential singer should be able to search through a list of songs by either the artist name, the title of the song, or the name of one of the contributors.
 A contributor is someone who has contributed to the creation of the song in some significant way, such as the author, the singer, the guitarist, the drummer, etc. As an example, this should allow a user to find all of the songs that Paul McCartney has made contributions to, whether it was as a member of The Beatles or as a member of Wings.

*( There needs to be information on what contribution each of these contributors has made for each song. As an example, David Bowie would have contributed as a writer, a singer, and likely a guitarist in most of his songs. There are, however, songs that he did not perform, but only wrote, like “All the Young Dudes”, which he wrote, but which was initially performed by a band called “Mott the Hoople”)*

Each song will have at least one karaoke file, or it wouldn’t be present on the list (because the karaoke presentation software wouldn’t have anything to play), but each song may possibly have many karaoke files, one for each of several possible versions. Each of these files will have a unique identifier. Since it may be important to the karaoke singer which version they are to perform, the version should also be a part of the information used when a user signs up in one of the queues to sing a song. 
*(As an example of multiple versions of a file, think of a duet. There may be a version that is arranged so that both partners get to sing, as well as a version for each of the parts, with the other singer’s part dubbed in (in case a singer wants to sing one part and doesn’t have a partner).

 Signing up to sing :
Upon choosing a version of a song, the user should be able to enter their request to sing a their chosen song into one of two queues that are stored separately. The first queue is a free for all, first come, first served queue that can be entered without charge. The other queue is an accelerated, priority queue, where the user can pay money to potentially have his song played earlier. Your application needs to allow people to sign up in the queues for singing. The DJ will decide how to actually choose which song plays next at any given time, but the contents of each of the queues should be shown to him separately. 

DJ interface :
You are also tasked with designing the DJ interface. This interface should show both queues separately (DO NOT MERGE THEM), but on the page, including relevant information about both the user that is singed up to sing and the version of the song they signed up in the queue to sing. This information should include the user who requested the song, its title, the name of the band that performed it, and the special karaoke file ID associated with the version of the song that was selected. 

Web Interface Requirements :
The interface for a user signing up to sing must be separate from the DJ interface. When searching for a songs, it is possible that there may be many rows of results returned. When this occurs, the user should be able to click on a table’s column heading to sort the results based on the data value represented by that column. The first click will sort the table in ascending order based on that column, then the next will sort in descending order, then back to ascending again, etc. This problem can be solved with PHP, but there are also other ways of handling it if you’d like to look into other, more dynamic options. The free queue should be sorted based on the time the user signed up; first in, first out. The accelerated queue should be able to be sorted in either time order or by the amount paid. Make sure to implement some mechanism to switch the sort order.
