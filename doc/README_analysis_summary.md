# Implementations Summary

## ST implementations

| implementation                | WC search | WC insert | WC delete | AC search hit | AC insert | AC delete | ordered it? | key i/f
| --------------                | --------- | --------- | --------- | ------------- | --------- | --------- | ----------- | -------
| seq search (unordered list)   |   N       |      N    |      N    |       N/2     |   N       |    N/2    |     no      | equals()
| binary search (ordered array) |  lg N     |      N    |      N    |      lg N     |  N/2      |    N/2    |    yes      | compareTo()
| BST                           |   N       |      N    |      N    |    1.38 ln N  | 1.38 lg N |     ?     |    yes      | compareTo()
| red-black BST                 | 2 lg N    |    2 lg N |    2 lg N |    1.00 ln N  | 1.00 lg N | 1.00 lg N |    yes      | compareTo()

* **WC** => worst-case cost (after N inserts)
* **AC** => average-case cost (after N random inserts)
* **ordered it** => ordered iterator