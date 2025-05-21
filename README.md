This is a To-do Web application built with Node.js and Express
it has JWT authentication, and uses Prisma as ORM. It features user
registration/login, protected CRUD operations required for todos, 
and supports both SQLite and PostgreSQL databases. The API includes proper validation,
error handling, and is dockerized for easy deployment. 

Dependencies


express: 4.18.2  

jsonwebtoken: 9.0.2  

bcrypt: 5.1.1  

prisma: 5.12.1   

cors: 2.8.5 

dotenv: 16.3.1 

Development

nodemon: 3.1.0 


Clone:

git clone https://github.com/shrey1982000/to_do.git

cd to_do



Dependencies:

npm install



Config:

cp .env.example .env



Migrations:

npx prisma migrate dev --name init



Start server:

npm run dev



Docker Deployment

docker-compose up -d --build



API Endpoints


POST	/auth/signup	Register new user	No

POST	/auth/login	Login and get JWT token	No

GET	/todos	Get all todos	Yes

POST	/todos	Create new todo	Yes
