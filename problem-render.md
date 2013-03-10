##Problem Render
There's some question if this should live in the WeBWorK API or some PG API or both
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
