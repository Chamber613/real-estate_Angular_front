[![GitHub Repo stars](https://github.com/Chamber613)

# real-estate-management

A online property management solution for real estate and
physical property management. This can include residential,
commercial, and land real estate. a software developed to
connect property managers and potential buyers.


<p align="center">
  <img src="frontend/resources/portfolio/home01.png" width="550" title="home" alt="Home">
  <img src="frontend/resources/portfolio/home05.png" width="550" title="home" alt="Home">
  <img src="frontend/resources/portfolio/home02.png" width="550" title="home" alt="Home">
  <img src="frontend/resources/portfolio/home04.png" width="550" title="home" alt="Home">
  <img src="frontend/resources/portfolio/home03.png" width="550" title="home" alt="Home">
</p>
🚧 **frontend/** work in progress 🚧.

🚧 **backend-fastify/** work in progress 🚧.


## **Dependencies**

### **Frontend**
- [Ionic 7+](https://ionicframework.com/)
- [Angular 16+](https://angular.io/)
- [leaflet 1.7+](https://leafletjs.com/)
- [chartjs 3.5+](https://www.chartjs.org/)

### **Backend**
- [Node](https://nodejs.org/en/)
- [fastify 4+](https://www.fastify.io/)
- [mongoDB](https://www.mongodb.com/)

# **SETUP**

## **Frontend (Part)**

### **1.1 navigate to `frontend/` directory.**

```
#  navigate to frontend 
$ cd frontend
```

### **1.2 Fill the desired environment variables:**  
- navigate to `frontend/src/environments`
- set values to variables (ex. api.url) 
```
  api: {
    url: 'http://localhost:8000/', <-- server URL
    mapKey: '', <-- Leaflet map key,
    googleAuthClientId: '', <-- google Auth CLient ID for Social signin
    webSocketUrl: 'ws://localhost:8000/websocket' <-- websocket URL
  }
```

### **2. then install dependencies & run ionic serve**

In terminal - command
```
# install dependencies
$ npm install

# serve frontend
$ ionic serve
```

<br>

## **Backend-Fastify (Part)**
### **1.1 navigate to `backend-fastify/` directory.**
```
cd backend-fastify/
```
### **1.2 create `.env` file & add variables:**
- copy `.env.example` & re-name it to `.env`
- set your desired variable value
```
PORT=8000
LOGGER=true
SALT=12
SECRET_KEY='secret'
DB_CONNECT=mongodb://localhost:27017/rem-db
```
### **2. then install dependencies & run dev**

In terminal - command
```
#  navigate to backend-fastify 
$ cd backend-fastify

# install dependencies
$ npm install

# start server
$ npm start `or` $ npm run dev

```

### **2.1 Database seeder(optional)**
- Make sure `.env` is configured & dependencies are installed
- Will populate database with dummy data.

⚠️ This will delete existing records in the database document. 

⚠️ Make a backup if needed
```
$ npm run db:seeder
```

dummy user:
```
  fullName: "test tester",
  email: "test@email.com",
  password: "password"

  You can use this to signin.
```
## Routes
```
/docs/
/users/
/auth/
/properties/
/enquiries/
```
