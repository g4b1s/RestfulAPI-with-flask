## First

```bash
$ pip install -r requirements.txt
```



## Usage

### Start server

```bash
./app.py

```

### rest methods 

###default GET 
```bash
curl -i http://localhost:5000
```

###GET
```bash
curl -i http://localhost:5000/todo/api/v1.0/tasks/1
```

###Auth GET 
```bash
curl -ugabriel:python -i http://localhost:5000/todo/api/v1.0/all_tasks/
```

###POST
```bash
curl -i -H "Content-Type: application/json" -X POST -d '{"title":"Read a book"}' http://localhost:5000/todo/api/v1.0/tasks
```

###PUT
```bash
curl -i -H "Content-Type: application/json" -X PUT -d '{"done":true}' http://localhost:5000/todo/api/v1.0/tasks/2
```

###DELTE
```bash
curl -i -H "Content-Type: application/json" -X DELETE  http://localhost:5000/todo/api/v1.0/tasks/3   
```
