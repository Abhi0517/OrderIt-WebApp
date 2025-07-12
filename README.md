# OrderIt-WebApp  – React + Node.js + MongoDB 
A full-stack online food-ordering website that allows users to browse a wide variety of menu-items, add them to their cart, place orders, and securely make online payments through *Stripe* payment gateway. The system also includes a password recovery feature via email through *MailTrap*.

## Features

### Customer-Facing Features
- **Browse & Order from a Large Menu**
  
  Menu items are dynamically loaded from *MongoDB*, offering multiple categories and rich details.
  
  <img width="1918" height="875" alt="Screenshot 2025-07-11 215546" src="https://github.com/user-attachments/assets/02a28efd-e654-470a-a0bc-a42cbf42492c" />
  <img width="1919" height="877" alt="Screenshot 2025-07-11 215754" src="https://github.com/user-attachments/assets/d01bda2a-f862-4ec7-9ec8-0cace1fab770" />
  
- **Add to Cart & Checkout**  

  Users can easily select items, view their cart, and update quantities before confirming the order.
  
  <img width="1918" height="875" alt="Screenshot 2025-07-11 215938" src="https://github.com/user-attachments/assets/f3c581c7-9b8b-42db-a4f9-a9133f24c1cd" />
  
- **Secure Stripe Payment Integration**
  
  Integrated with *Stripe API* for fast, reliable, and secure online payments.
  
  <img width="1918" height="874" alt="Screenshot 2025-07-11 220024" src="https://github.com/user-attachments/assets/4896cf27-c9aa-413f-99a1-ac634658eef8" />
  <img width="1917" height="880" alt="Screenshot 2025-07-11 220211" src="https://github.com/user-attachments/assets/92852823-5197-4f80-bf1e-282026fc0298" />
  <img width="1919" height="882" alt="Screenshot 2025-07-11 220227" src="https://github.com/user-attachments/assets/73de309f-c668-498e-98bf-dd0ee46939f6" />
  <img width="1918" height="876" alt="Screenshot 2025-07-11 220320" src="https://github.com/user-attachments/assets/0ce948c1-e0ee-49a4-8619-347c8de360f0" />

- **Upload Food Images with Cloudinary**  
  Admins or users can upload images via *Cloudinary*, enabling high-performance image hosting and on-the-fly transformations.

- **Authentication & Forgot Password**  
  Users can sign up, log in, and reset forgotten passwords through an email-based flow powered by *Mailtrap* (for dev/testing).

## Tech Stack

| Layer        | Technology             |
|--------------|------------------------|
| Frontend     | React, Redux Toolkit   |
| Backend      | Node.js, Express       |
| Database     | MongoDB + Mongoose     |
| Payments     | Stripe API             |
| Image Upload | Cloudinary             |
| Email Service| Mailtrap (SMTP dev env)|
| State Mgmt   | Redux Toolkit + React Redux |

## Getting Started

### 1. Clone the Repo
```Powershell
git clone https://github.com/your-username/your-repo.git
cd "FoodOrder\frontend"
```
### 2. Install Dependencies
```Powershell
npm install
```
### 3. Start the Development Server
Split the terminal, one for *FoodOrder\frontend* and another for *FoodOrder\Backend-obfuscated*:
```Powershell
npm start
```
### 4. Configure Environment Variables
For backend:
```Powershell
CLOUDINARY_CLOUD_NAME=cloud_name
CLOUDINARY_API_KEY=cloudinary_api_key
CLOUDINARY_API_SECRET=cloudinary_api_secret
DB_LOCAL_URI=your_mongo_db_connection_string
EMAIL_USERNAME=mailtrap_username
EMAIL_PASSWORD=mailtrap_password
STRIPE_SECRET_KEY=your_stripe_key
STRIPE_API_KEY=your_stripe_api_key
```
## Points To Remember
- Password reset emails are routed via Mailtrap (safe for dev testing).
- You can extend the app with admin features like:
     - Order management
     - Menu item management
     - Analytics dashboard
## Feel free to fork and contribute !!
