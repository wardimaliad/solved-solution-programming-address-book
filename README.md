Download Link: https://assignmentchef.com/product/solved-solution-programming-address-book
<br>
Programming: Address book SolutionYou will implement a Java console application that manages a simple address book. The address book consists of a list of contacts, and it provides methods to add, find, and print those contacts. Each contact consists of only a name and a phone number.

The address book initially contains no contacts, and the application never saves or loads any data to or from permanent storage.

You must implement the address book as a Java class named AddressBook, and you must implement individual contact information as a Java class named Contact. The AddressBook should contain a collection of Contact instances. The following class diagram depicts this relationship:

Address Book

-contacts: List

—————————–

+add (c: Contact) : void

+find (s: String): List &lt; Contact

+toString (): String

Contact

——–

-name: String

-phone: String

————–

+to String (): String

The application operates in a loop. For each iteration, the application first shows a menu of available commands, then prompts the user to enter a command, and then finally processes that user-supplied command

Start show menu prompt user quit? end ( repeat)

The menu of available commands and the prompt presented to the user appear as follows:

~ Address Book Menu ~

+————————-


ADD Adds a contact

FIND Finds contacts

PRINT Prints contacts

QUIT Quits

+————————-


—

The user may enter one of the following commands: add, find, print, or quit. The application ignores letter case when determining the command. If the user enters an invalid command, the application responds by writing “Invalid command.” and looping. For example, if the user enters “upload”, the application responds as follows:

Adding Contacts

If the user enters the command add, the application prompts the user for a name and a phone number. The user may enter any non-empty strings for these values. After the user enters the two values, the application displays a message indicating the successful addition of the contact to the address book. The following demonstrates this interaction:

— add

NAME — Henry Ford

PHONE — 808-544-0862

Added [Heny Ford; 808-544-0862]

Finding Contacts

If the user enters the command find, the application prompts the user for text it will use to search the address book. The user may enter any non-empty string for this value. After the user enters the text, the application displays a list of all contacts that contain that text in either the contact�s name or phone number. The application ignores letter case when performing this search. After displaying all matching contacts, the application displays the number of contacts found. The following demonstrates this interaction:

— find

WHAT — 808

[Mike Myers; 808-544-0862]

[Curt Powley; 808-544-1145]

3. Printing the Address Book

If the user enters the command print, the application prints a list of all contacts in the address book, followed by the number of contacts it printed. The following demonstrates this interaction:

— print

[Peter Doe; 206-2523]

[Chris Pratt; 808-544-0813]

[Curt Powley; 808-544-1145]

Number of contacts: 3

4. Quitting

When the user enters the command quit, the application terminates without displaying any additional messages. The following demonstrates this interaction:

— quit

$java Mike Myers2

~ Address Book Menu ~

+————————-


ADD Adds a contact

FIND Finds contacts

PRINT Prints contacts

QUIT Quits

+————————-


— add


