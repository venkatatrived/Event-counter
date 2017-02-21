# Event-counter
Event counter using red-black tree data structure. Each event has two fields ID and Count. Count field maintains the number of active events with given ID. The counter should support Increase, Reduce, Count, InRange, Next and Previous operations in the specified time complexity.

• Increase takes id and m as input arguments. If id is present in the event counter tree, it increases the count of given id by m or creates a new event with given arguments and insert it into the tree. Time Complexity: O(log n)

• Reduce takes id and m as input arguments. If id is present in the event counter tree, it reduces the count of given id by m. After reduction if count is less than zero, it removes the Id from the event counter tree. Time Complexity: O(log n)

• Count takes id as input argument and returns the count of the event with given id, if it is present in the event counter tree. Time Complexity: O(log n)

• InRange takes id1 and id2 as input argument and returns the sum of all the counts of events with ids between id1 and id2 inclusively. Time Complexity: O(log n + s), where s is the number of IDs in the given range.

• Next takes id as input arguments and returns the next event with lowest id that is greater that of given id. Time Complexity: O(log n)

• Previous takes id as input arguments and returns the next event with greatest id that is less than the given id. Time Complexity: O(log n)
