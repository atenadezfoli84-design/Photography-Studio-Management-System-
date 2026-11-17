# Photography-Studio-Management-System-Activity 3: Architecture and API Contract
Architecture: Modular Monolith (Auth, Users, Bookings connected to one Database).
​API Contract:
POST /api/users
GET /api/users/:id
POST /api/bookings
GET /api/bookings
PUT /api/bookings/:id/cancel
​Activity 4: Docker Commands
docker build -t photography-api .
docker run -d -p 3000:3000 --name photo-api-container photography-api

