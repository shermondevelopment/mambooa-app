# <p align = "center"> KANBAM MAMBOO </p>

<p align="center">
   <img src="https://mamboo.co.ao/images/logo/logo-dark.png" width="150"/>
</p>

## :clipboard: Description

create a system where I can create my board and within these boards I can have several lists and in this list I can link several tasks to them

---

## :computer: Technologies

- TypeScript
- Node.js
- MongoDb
- JWT
- Bcrypt

## Instructions on how to run with Docker

<p>
  You need to have installed the following tools: Git, Docker, Docker Compose. It will be necessary for port 3001 to be available for the application and mongodb will use port 27017.
</p>


<p>
 then go up the application's docker container:
</p>

```yml
docker-compose up -d
```

<p>
 App FrontEnd running in port 80 
</p>

```yml
http://localhost
```

<p>
 App BackEnd running in port 3001
</p>

```yml
http://localhost:3001
```


## :rocket: Routers of List

```yml
POST /new/list
    - Route to register a new list
    - headers: {}
    - body:
        {
          "title": "To Do"
        }
```

```yml
PUT /update/list/:id_list
    - Route to update list
    - headers: {}
    - body:
        {
            "title" "To do 2"
        }
```

```yml
DELETE /delete/list/:id_list
    - Route to delete list
    - headers: {}
    - body: {}
```

```yml
GET /get/list
    - Route to get list
    - headers: {}
    - body: {}
```

## Routers of cards

```yml
POST /card
    - Route to create new card
    - headers: {  }
    - body:
        {
            "content": "My frame Kanbam",
            "list_id": "uuid"
        }
```

```yml
PUT /card 
    - Route to updated card
    - headers: {  }
    - body: {
        "content": "My frame Kanbam",
        "list_id": "uuid"
    }
```

```yml
DELETE /card/?id_card
    - Route to delete card
    - headers: {  }
    - body: {}
```

```yml
GET /cards
    - Route to list cards
    - headers: {  }
    - body: {}
```
