NoSQL

This project contains tasks for learning to use the MongoDB NoSQL database application.

Tasks To Complete

 0. List all databases
0-list_databases contains a MongoDB script that lists all databases in MongoDB.

 1. Create a database
1-use_or_create_database contains a MongoDB script that creates or uses the database my_db.

 2. Insert document
2-insert contains a MongoDB script that inserts a document in the collection school:

The document must have one attribute name with value “Holberton school”.
The database name will be passed as an option of mongo command.
 3. All documents
3-all contains a MongoDB script that lists all documents in the collection school:

The database name will be passed as an option of mongo command.
 4. All matches
4-match contains a MongoDB script that lists all documents with name="Holberton school" in the collection school:

The database name will be passed as an option of mongo command.
 5. Count
5-count contains a MongoDB script that displays the number of documents in the collection school:

The database name will be passed as an option of mongo command.
 6. Update
6-update contains a MongoDB script that adds a new attribute to a document in the collection school:

The script should update only document with name="Holberton school" (all of them).
The update should add the attribute address with the value “972 Mission street”.
The database name will be passed as an option of mongo command.
 7. Delete by match
7-delete contains a MongoDB script that deletes all documents with name="Holberton school" in the collection school:

The database name will be passed as an option of mongo command.
 8. List all documents in Python
8-all.py contains a Python function that lists all documents in a collection:

Prototype: def list_all(mongo_collection):.
Return an empty list if no document in the collection.
mongo_collection will be the pymongo collection object.
 9. Insert a document in Python
9-insert_school.py contains a Python function that inserts a new document in a collection based on kwargs:

Prototype: def insert_school(mongo_collection, **kwargs):.
mongo_collection will be the pymongo collection object.
Returns the new _id.
 10. Change school topics
10-update_topics.py contains a Python function that changes all topics of a school document based on the name:

Prototype: def update_topics(mongo_collection, name, topics):.
mongo_collection will be the pymongo collection object.
name (string) will be the school name to update.
topics (list of strings) will be the list of topics approached in the school.
 11. Where can I learn Python?
11-schools_by_topic.py contains a Python function that returns the list of school having a specific topic:

Prototype: def schools_by_topic(mongo_collection, topic):.
mongo_collection will be the pymongo collection object.
topic (string) will be topic searched.
 12. Log stats
12-log_stats.py contains a Python script that provides some stats about Nginx logs stored in MongoDB:

Database: logs.
Collection: nginx.
Display:
First line: x logs where x is the number of documents in this collection.
Second line: Methods:.
5 lines with the number of documents with the method = ["GET", "POST", "PUT", "PATCH", "DELETE"] in this order (see example below - warning: it’s a tabulation at the start of each line).
One line with the number of documents with:
method=GET.
path=/status.
Example:
94778 logs
Methods:
    method GET: 93842
    method POST: 229
    method PUT: 0
    method PATCH: 0
    method DELETE: 0
47415 status check
You can use this dump as data sample: dump.zip.
 13. Regex filter
100-find contains a MongoDB script that lists all documents with name starting by Holberton in the collection school:

The database name will be passed as an option of the mongo command.
 14. Top students
101-students.py contains a Python function that returns all students sorted by average score:

Prototype: def top_students(mongo_collection):.
mongo_collection will be the pymongo collection object.
The top must be in descending order of average score.
The average score must be part of each item returns with key = averageScore.
A sample document in the collection is shown below:
{
  "name": "Julia",
  "topics": [
    { "title": "Algo", "score": 10.5 },
    { "title": "C", "score": 10.2 },
    { "title": "Python", "score": 10.1 }
  ]
}
 15. Log stats - new version
102-log_stats.py improves 12-log_stats.py by adding the top 10 of the most present IPs in the collection nginx of the database logs:

The top 10 IPs must be sorted.
