# FastAPI Basic Auth Backend

This is a simple FastAPI backend application that demonstrates basic authentication functionality using FastAPI's built-in `HTTPBasic` security scheme.

## Installation

1. Clone the repository:

   ```bash
   https://github.com/NicolasR98/fastapi-basic-auth
   ```

2. Navigate to the project directory:

   ```bash
   cd fastapi-basic-auth-backend
   ```

3. Create a virtual environment (optional but recommended):

   ```bash
   python3 -m venv env
   source env/bin/activate
   ```

4. Install the dependencies:

   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. Run the FastAPI application:

   ```bash
   uvicorn main:app --reload
   ```

   This will start the FastAPI server locally.

2. Open your web browser and navigate to `http://localhost:8000/docs` to access the interactive API documentation (provided by Swagger UI).

3. You can now try out the available endpoints, including the `/login` endpoint for authentication.

4. To access the protected endpoint `/protected`, provide the username and password when prompted (using Basic Auth) using the credentials of a valid user. Alternatively, you can also pass the credentials using the "Authorize" button in the Swagger UI.

   - Username: `user`
   - Password: `password`

5. If the credentials are valid, you will receive a successful response from the `/protected` endpoint. Otherwise, you will receive a 401 Unauthorized response.
