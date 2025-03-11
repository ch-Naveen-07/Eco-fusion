EcoFusion: AI-Powered Waste Management System
EcoFusion is an AI-driven platform designed to optimize waste collection and recycling in the agricultural sector. The project focuses on converting agricultural waste into eco-friendly fuel, such as briquettes, while reducing the environmental impact caused by the burning of waste. By utilizing artificial intelligence for waste sorting, route optimization for collection trucks, and real-time notifications, EcoFusion aims to create a more sustainable agricultural ecosystem.

Key Features
1. AI-Powered Waste Classification
Uses Hugging Face for real-time classification of agricultural waste images (such as straw, husks, and plastic).
Helps farmers properly categorize waste for recycling and fuel conversion.
2. Route Optimization
Implements GraphHopper to optimize waste collection truck routes.
Reduces fuel consumption and transportation costs while ensuring timely collection.
3. Real-time Email Notifications
Uses the Resend API to send email notifications to both farmers and waste collection drivers.
Ensures seamless communication about collection schedules, waste status, and updates.
4. Impact Dashboard
Provides a dashboard to visualize the environmental impact of the project.
Tracks metrics such as carbon savings, waste reduction, and the number of pickups completed.
5. User Authentication & Admin Panel
Secure login system with role-based access for farmers, waste collectors, and admins.
Farmers can upload waste images, and collectors can view and manage their routes.
6. Modern UI with TailwindCSS & React
Built with React and styled using TailwindCSS, providing a responsive and clean interface.
Designed for a seamless experience across desktop and mobile devices.
Technologies Used
Frontend: React, TailwindCSS
Backend: Node.js, Supabase (for database and authentication)
AI: Hugging Face (for image classification)
Route Optimization: GraphHopper API
Email Notifications: Resend API
How It Works
Farmers upload images of agricultural waste via the app.
AI classifies the type of waste (e.g., straw, plastic).
Waste collection routes are optimized using real-time data and GraphHopper API.
Collection trucks follow the optimized routes and collect the waste from farmers.
Environmental impact metrics (e.g., carbon savings) are tracked and displayed in the dashboard.
Real-time notifications are sent to farmers and drivers via email.
Installation & Setup
To run EcoFusion locally, follow these steps:

1. Clone the Repository
bash
Copy code
git clone https://github.com/your-username/ecofusion.git
2. Install Dependencies
Navigate to the project folder and run the following command to install all required dependencies:

bash
Copy code
npm install
3. Set Up Environment Variables
Create a .env file in the root of the project and add the following environment variables:

env
Copy code
VITE_SUPABASE_URL=your_supabase_url
VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
VITE_RESEND_API_KEY=your_resend_api_key
VITE_HUGGINGFACE_API_KEY=your_huggingface_api_key
Make sure to replace the placeholders with your actual API keys.

4. Run the Development Server
After setting up the environment variables, start the development server with:

bash
Copy code
npm run dev
Visit http://localhost:5173/ to view the project.

Project Structure
The directory structure of the EcoFusion project is as follows:

bash
Copy code
ecofusion/
│
├── public/                    # Public assets (images, fonts, etc.)
├── src/                       # Source files
│   ├── components/            # React components
│   ├── lib/                   # Helper functions and APIs
│   ├── App.js                 # Main app component
│   ├── index.js               # Entry point for React
│   └── styles/                # TailwindCSS custom styles
├── .env                       # Environment variables
├── package.json               # NPM package file
├── postcss.config.js          # PostCSS configuration for Tailwind
├── tailwind.config.js         # Tailwind configuration
└── vite.config.ts             # Vite configuration
Contributing
If you'd like to contribute to EcoFusion, follow these steps:

Fork the repository.
Create a new branch (git checkout -b feature-name).
Make your changes and commit them (git commit -am 'Add feature').
Push to your branch (git push origin feature-name).
Create a new Pull Request.

Contact
If you have any questions or would like to discuss improvements to the project, feel free to reach out!
