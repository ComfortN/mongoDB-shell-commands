# MongoDB Project README

This README provides instructions on how to start the MongoDB shell (mongosh) and outlines the specific MongoDB shell commands used to achieve the project outcomes.

## Starting MongoDB Shell

1. Ensure MongoDB is installed on your system.
2. Open a terminal or command prompt.
3. Type `mongosh` and press Enter to start the MongoDB shell.

## Project Commands

### Create Database

```
use Codetribe
```

This command creates (if it doesn't exist) and switches to the Codetribe database.

### Create Collections

The collections will be created automatically when we insert documents into them. No specific command is needed to create collections.

### Insert Documents

1. Insert a document into the Facilitators collection:

```
db.Facilitators.insertOne({
  Name: "Mahlatse Serathi",
  Location: "Soweto",
  Course: "Web Development"
})
```

2. Insert a document into the Trainees collection:

```
db.Trainees.insertOne({
  Name: "Comfort Ngwenya",
  Location: "Soweto",
  Facilitator: "Mahlatse Serathi"
})
```

3. Insert a document into the Projects collection:

```
db.Projects.insertOne({
  Name: "MongoDB task 2",
  Course: "Web Development",
  Lesson: "MongoDB"
})
```

### Verify Insertions

To verify that the documents have been inserted correctly, you can use the following commands:

1. View all documents in the Facilitators collection:

```
db.Facilitators.find()
```

2. View all documents in the Trainees collection:

```
db.Trainees.find()
```

3. View all documents in the Projects collection:

```
db.Projects.find()
```

