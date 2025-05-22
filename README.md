This is a To-do Web application built with Node.js and Express
it has JWT authentication, and uses Prisma as ORM. It features user
registration/login, and has protected CRUD operations required for todos, 
it also supports both SQLite and PostgreSQL databases. The API includes proper validation,
error handling, and is dockerized for easy deployment. 

**Dependencies**



express: 4.18.2  

jsonwebtoken: 9.0.2  

bcrypt: 5.1.1  

prisma: 5.12.1   

cors: 2.8.5 

dotenv: 16.3.1 

**Development**

nodemon: 3.1.0 


**Clone:**

clone this repo



**Dependencies:**

npm install



**Config:**

cp .env.example .env



**Migrations:**

npx prisma migrate dev --name init



**Start server:**

npm run dev



**Docker Deployment**

docker-compose up -d --build



**API Endpoints**


POST	/auth/signup	Registers new user	No auth req

POST	/auth/login	Logs in and gets JWT token	No auth req

GET	/todos	Gets all todos	Auth req

POST	/todos	Creates new todo	Auth req
