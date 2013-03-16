##Problem Render
This needs to exist in both the webwork server and in PG.  
The webwork server will request rendering and check answers using PG's API
The reason for the redundancy is that PG shouldn't care about state when checking answers whereas WeBWorK needs to record attempts etc.

###get rendered (id, path, code)  
```
GET /problem
```
body contains id, path, code
###check answer (id, path, code)  
```
POST /problem/check
```
body contains id, path, code and answer
###create (code?)  
```
POST /problem/create
```
body contains code (maybe path?)
