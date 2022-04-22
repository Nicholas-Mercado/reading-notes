# Implementation: Linked Lists

Linked Lists are sort of like a group of people who can do two things. First they can hold a piece of data and second they know and can point to the next person in the queue.

This is a huge advantage over a queue of people lined up in a row. Say you want to remove or add someone from the center of the line. One person enters the line but now every one has to move one to the right left to make room in the line.

This is not so with the group of people using linked list. Say you want to add a new person to the queue between person six and person seven. All you you have to do is tell person six to point to the new person and new person to point to person seven. Tad dah! You have now added to the queue with out having to make the whole line move.  

## disadvantages

- slow to get to a element
- linear or O(n)

## advantages

- Insert and deleted can be quick
- Elements can be unsorted or sorted
- Lists can have duplicates
- No pre allocation of space needed

