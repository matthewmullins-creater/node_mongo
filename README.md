# Node.js Express + MongoDB User API

## Setup

1. **Install dependencies:**
   ```sh
   npm install
   ```

2. **Configure MongoDB:**
   - Set your MongoDB connection string in the `.env` file:
     ```
     MONGODB_URI=mongodb://localhost:27017/yourdbname
     ```

3. **Start the server:**
   ```sh
   node index.js
   ```

## API Usage

### GET `/users/:id`
- Returns user details in JSON if found and age > 21.
- Returns 404 if not found or age <= 21.
- Returns 400 if the id is invalid.

#### Example Response
```json
{
  "_id": "...",
  "name": "John Doe",
  "email": "johndoe@email.com",
  "age": 30
}
``` 