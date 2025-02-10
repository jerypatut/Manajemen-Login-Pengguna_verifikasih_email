# Login and Registration Application

This application provides a login and registration system with two user roles: **Admin** and **User**. Admins have full access to edit data, while Users have limited access. After registration, users will receive a confirmation email before being able to log in.

## Technologies Used

- **Backend**: Node.js, Express.js  
- **Database**: MongoDB  
- **Frontend**: React.js  

## Key Features

### 1. **Home Page**
   - The main page of the application with general information.
   - Screenshots:  
     ![Home Page](/scrinsut/beforelogin.png)  
     ![After Login](/scrinsut/sudahverifikasih.png)  

### 2. **Login Page**
   - Users can log in using their registered email and password.  
     ![Login Page](/scrinsut/loginkerja.png)  

### 3. **Register Page**
   - New users can register by filling in their name, email, and password.
   - After registration, users will receive an email confirmation with a verification code. Only verified users can log in.  
     ![Register Page](/scrinsut/registerconfimasion.png)  
     ![Email Verification Page](/scrinsut/verifikasihemail.png)  
     ![Verification Success Page](/scrinsut/verifikasih.png)  

### 4. **Forgot Password Page**
   - Users can reset their password by entering their registered email. A confirmation code will be sent via email.  
     ![Forgot Password Page](/scrinsut/resetpassword.png)  

### 5. **Email Confirmation Page**
   - After registration, users must confirm their account via email before logging in.  
     ![Email Confirmation Page](/scrinsut/verifikasih.png)  

## Steps to Run the Application

1. **Clone the Repository**

   ```bash
   git clone <repository-url>
   cd project-directory
   ```

2. **Install Dependencies**

   ```bash
   # Install backend dependencies
   cd backend
   npm install

   # Install frontend dependencies
   cd ../frontend
   npm install
   ```

3. **Configure Environment Variables**
   Create a `.env` file in the `backend` directory and add the following configuration:

   ```env
   MONGO_URI=mongodb://127.0.0.1:27017/login_app
   PORT=5000
   JWT_SECRET=your_jwt_secret
   EMAIL_HOST=smtp.gmail.com
   EMAIL_USER=your-email@gmail.com
   EMAIL_PASS=your-email-password
   ```

   Create a `.env` file in the `frontend` directory and add the following configuration:

   ```env
   REACT_APP_API_URL=http://localhost:5000
   ```

4. **Run the Application**

   ```bash
   # Run backend
   cd backend
   npm start

   # Run frontend
   cd ../frontend
   npm start
   ```

5. **Access the Application**
   Open a browser and navigate to [http://localhost:3000](http://localhost:3000).

## Project Structure

```
/project-directory
|-- /backend
|-- /frontend
|-- /scrinsut
|-- readme.md
```

## Upcoming Features

- Reset password using OTP.
- Enhanced user interface design.
- Admin dashboard for user data management.

---
Developed by **jeripatut**.
