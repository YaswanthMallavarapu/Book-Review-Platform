<!DOCTYPE html>
<html>
<body>
  <h1 align="center">📚 Book Review Platform</h1>
  
  <p align="center">
    <img src="https://img.shields.io/badge/React-18.2.0-blue" alt="React">
    <img src="https://img.shields.io/badge/Vite-4.3.2-purple" alt="Vite">
    <img src="https://img.shields.io/badge/Node.js-Express-green" alt="Express">
    <img src="https://img.shields.io/badge/MongoDB-Latest-green" alt="MongoDB">
    <img src="https://img.shields.io/badge/Tailwind-3.3.1-blue" alt="Tailwind">
  </p>
  
  <p align="center">
    A full-stack web application for book enthusiasts to discover, review, and rate books.
    <br />
    <a href="#demo"><strong>View Demo »</strong></a>
    <br />
    <br />
    <a href="#features">Features</a> •
    <a href="#tech-stack">Tech Stack</a> •
    <a href="#installation">Installation</a> •
    <a href="#usage">Usage</a> •
    <a href="#api-endpoints">API Endpoints</a> •
    <a href="#contributing">Contributing</a> •
    <a href="#license">License</a>
  </p>
  
  <hr />
  
  <h2 id="features">✨ Features</h2>
  
  <ul>
    <li><strong>User Authentication</strong> - Register, login, and profile management</li>
    <li><strong>Book Browsing</strong> - View featured books and browse the complete collection</li>
    <li><strong>Search & Filter</strong> - Find books by title, author, genre, or rating</li>
    <li><strong>Book Details</strong> - View comprehensive information about each book</li>
    <li><strong>Review System</strong> - Read and write reviews for books</li>
    <li><strong>Rating System</strong> - Rate books on a scale of 1-5 stars</li>
    <li><strong>User Profiles</strong> - View and manage your reviews</li>
    <li><strong>Responsive Design</strong> - Optimized for both desktop and mobile devices</li>
  </ul>
  
  <h2 id="tech-stack">🛠️ Tech Stack</h2>
  
  <h3>Frontend</h3>
  <ul>
    <li>React.js with Vite</li>
    <li>React Router for navigation</li>
    <li>Context API for state management</li>
    <li>Tailwind CSS for styling</li>
    <li>Lucide React for icons</li>
  </ul>
  
  <h3>Backend</h3>
  <ul>
    <li>Node.js with Express</li>
    <li>MongoDB for database</li>
    <li>JWT for authentication</li>
    <li>Bcrypt for password hashing</li>
  </ul>
  
  <h2 id="installation">🔧 Installation</h2>
  
  <h3>Prerequisites</h3>
  <ul>
    <li>Node.js (v14 or higher)</li>
    <li>MongoDB (local or Atlas URI)</li>
    <li>Git</li>
  </ul>
  
  <h3>Clone the Repository</h3>
  <pre><code>git clone https://github.com/YaswanthMallavarapu/Book-Review-Platform.git
cd book-review-platform</code></pre>
  
  <h3>Backend Setup</h3>
  <pre><code># Navigate to server directory
cd server

# Install dependencies

npm install

# Create .env file with the following variables

# MONGODB_URI=mongodb+srv://&lt;db_username&gt;:&lt;db_password&gt;@cluster0.uruty9i.mongodb.net/bookreview

# JWT_SECRET=your_jwt_secret_key

# PORT=5000

# Seed the database with sample data (optional)

npm run seed

# Start the server

npm run dev</code></pre>

  <h3>Frontend Setup</h3>
  <pre><code># Navigate to client directory
cd ../client

# Install dependencies

npm install

# Start the development server

npm run dev</code></pre>

  <p>The application will be available at <a href="http://localhost:3000">http://localhost:3000</a>, with the backend API running at <a href="http://localhost:5000">http://localhost:5000</a>.</p>
  
  <h2 id="usage">📖 Usage</h2>
  
  <h3>User Registration and Login</h3>
  <ol>
    <li>Navigate to the Register page to create a new account</li>
    <li>Use your credentials to log in</li>
    <li>Once logged in, you can access your profile and submit reviews</li>
  </ol>
  
  <h3>Browsing Books</h3>
  <ol>
    <li>The home page displays featured books</li>
    <li>Navigate to the Books page to see all available books</li>
    <li>Use the search bar and filters to find specific books</li>
  </ol>
  
  <h3>Reading and Writing Reviews</h3>
  <ol>
    <li>Click on a book to view its details and reviews</li>
    <li>If logged in, you can submit your own review and rating</li>
    <li>View all your reviews in your profile page</li>
  </ol>
  
  <h2 id="api-endpoints">🔌 API Endpoints</h2>
  
  <h3>Authentication</h3>
  <ul>
    <li><code>POST /api/users/register</code> - Register a new user</li>
    <li><code>POST /api/users/login</code> - Login a user</li>
    <li><code>GET /api/users/me</code> - Get current user (requires authentication)</li>
  </ul>
  
  <h3>Books</h3>
  <ul>
    <li><code>GET /api/books</code> - Get all books (with pagination and filtering)</li>
    <li><code>GET /api/books/featured</code> - Get featured books</li>
    <li><code>GET /api/books/:id</code> - Get a specific book</li>
    <li><code>POST /api/books</code> - Add a new book (admin only)</li>
    <li><code>PUT /api/books/:id</code> - Update a book (admin only)</li>
    <li><code>DELETE /api/books/:id</code> - Delete a book (admin only)</li>
  </ul>
  
  <h3>Reviews</h3>
  <ul>
    <li><code>GET /api/reviews?bookId=:bookId</code> - Get reviews for a book</li>
    <li><code>GET /api/reviews/user</code> - Get reviews by current user</li>
    <li><code>POST /api/reviews</code> - Add a new review</li>
    <li><code>PUT /api/reviews/:id</code> - Update a review</li>
    <li><code>DELETE /api/reviews/:id</code> - Delete a review</li>
  </ul>
  
  <h3>Users</h3>
  <ul>
    <li><code>PUT /api/users/:id</code> - Update user profile</li>
    <li><code>POST /api/users/change-password</code> - Change password</li>
  </ul>
  
  
  
  <h2 id="contributing">🤝 Contributing</h2>
  
  <p>Contributions are welcome! Please feel free to submit a Pull Request.</p>
  
  <ol>
    <li>Fork the Project</li>
    <li>Create your Feature Branch (<code>git checkout -b feature/AmazingFeature</code>)</li>
    <li>Commit your Changes (<code>git commit -m 'Add some AmazingFeature'</code>)</li>
    <li>Push to the Branch (<code>git push origin feature/AmazingFeature</code>)</li>
    <li>Open a Pull Request</li>
  </ol>
  
  <h2 id="license">📝 License</h2>
  
  <p>Distributed under the MIT License. See <code>LICENSE</code> for more information.</p>
  
  <hr />
  
  <p align="center">
    Made with ❤️ by <a href="https://github.com/YaswanthMallavarapu">Yaswanth Mallavarapu</a>
  </p>
</body>
</html>
