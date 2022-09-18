## Desafío Reformar API con GraphQL

Simple API con GraphQL using Nodejs and Mongodb

### Requerimentos

- Mongodb
- Nodejs

### Environment variables

```
  MONGO_URI
 
```

### Installation

```
npm i
npm start
npm dev 
```

### Consultas en ApolloServerGraphQL

`query{
	getAllTasks {
	    id 
	    title
	    description
    }
}`

`query {
	getTask(id: "aca_va_el_id_que_viene_desde_mongoDB"){
	    id
	    title
	    description
    }
} `

`mutation {
	createTask(
		task:{
		    title: "Mi Nueva Tarea",
		    description: "Nueva Tarea" 
		}
	)

} `

`mutation {
	deleteTask(id: "aca_va_el_id_que_viene_desde_mongoDB")
}`

`mutation {
	updateTask(
	    id: "aca_va_el_id_que_viene_desde_mongoDB"
	    task: {
	           title: "Actualizar title",
	           description: "Tarea actualizada"
	    })	
    {
	    id 
	    title
	    description
    }
}`

