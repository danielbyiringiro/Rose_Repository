## Shortest Path

The goal of this exercise is to link two actors `source` and `target` using the movies they acted in. You are provided with a folder called `data`. `data` contains three csv files. The first csv file is called movies.csv and contains three columns. The first column is id, which denotes the movie id, the second column is title which denotes the title of the movie and the third column is year which denotes when the movie was released. The second csv file is people.csv which also contains three columns id, name and birth denoting the actor id, their name and the year they were born respectively. The third csv file is called stars.csv and contains only two columns, the first is person_id followed by movie_id. An entry (person_id, movie_id) indicates that the actor with the indicated person_id acted in the movie with the indicated movie_id.

### Tasks

#### Task 1.1
You are to find the link between two actors using the movies they acted in. For example given Jennifer Lawrence as the source and Tom Hanks as the target one of the possible response is

- Jennifer Lawrence is connected to Kevin Bacon by both starring in "X-Men: First Class"
- Kevin Bacon is connected to Tom Hanks by both starring in "Apollo 13"

The degree of their connection is 2 [If they had acted in the same movie together their degree of connection would be 1]

You are to implement the code to solve this task in `depthfirst.py`, using the depth-first search technique.
The depth-first approach relies on a stack data structure.

#### Task 1.2
Same as Task 1.1 but the code to solve this task should be implemented in `breadthfirst.py`, using the breadth-first search technique. The breadth-first technique relies on a queue data structure.

### Notes
Functions common to both Task 1.1 and Task 1.2 should be implemented in `util.py` and imported in the respective files rather than being duplicated. Both `depthfirst.py` and `breadthfirst.py` should take in the `source` and `target` as command line arguements. 