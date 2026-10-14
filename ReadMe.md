# SkillRise

**A Learning and Career Development Platform**

SkillRise is a web-based learning and career development platform designed to help users organize their learning journey, explore career opportunities, manage projects, and track their progress.

## Features

- User Authentication
- User Profile Management
- Learning Roadmaps
- Project Management
- Career Development Support
- Progress Tracking
- REST API Integration
- React-Based User Interface
- MongoDB Database Integration

*Note: Confirm each feature against the current implementation before publishing this README.*

## Technology Stack

### Frontend
- React
- Vite
- JavaScript
- CSS

### Backend
- Node.js
- Express.js, if used by the backend
- MongoDB
- REST APIs

## Project Structure

```text
SkillRise/
├── Backend/
│   ├── config/
│   ├── controller/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   ├── package.json
│   └── server.js
│
├── skillrise-web/
│   ├── public/
│   ├── src/
│   │   ├── assets/
│   │   ├── pages/
│   │   ├── App.jsx
│   │   ├── App.css
│   │   └── main.jsx
│   ├── package.json
│   └── vite.config.js
│
├── .gitignore
└── ReadMe.md
```

## Requirements

Before running the project, install:

- Node.js and npm
- Git
- MongoDB or a MongoDB Atlas account
- Visual Studio Code or another code editor

## Clone the Repository

```bash
git clone https://github.com/tayyabsajjad76/SkillRise.git
cd SkillRise
```

## Backend Setup

Navigate to the backend directory:

```bash
cd Backend
npm install
```

### Environment Variables

Create a `.env` file inside the `Backend/` directory.

Add the environment variables required by your application. For example:

```env
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_strong_random_secret
PORT=5000
```

Use the exact variable names expected by your backend code. The values above are placeholders, not working credentials.

**Security:** Never commit `.env` files, database passwords, JWT secrets, or API keys to GitHub.

### Start the Backend

Use the command configured in `Backend/package.json`. If the project defines a `start` script, run:

```bash
npm start
```

If it defines a `dev` script, you can use:

```bash
npm run dev
```

## Frontend Setup

Open a second terminal and navigate to the frontend directory from the project root:

```bash
cd skillrise-web
npm install
```

### Start the Development Server

```bash
npm run dev
```

Vite will display a local development URL in the terminal. Open that URL in your browser.

## Running the Full Application

1. Configure the required backend environment variables.
2. Start the backend server.
3. Start the frontend development server in a separate terminal.
4. Ensure the frontend API configuration points to the correct backend URL.
5. Open the frontend URL in your browser.

## Common Commands

### Backend

```bash
npm install
npm start
npm run dev
```

Run only the commands supported by the scripts defined in `Backend/package.json`.

### Frontend

```bash
npm install
npm run dev
npm run build
npm run preview
```

## Troubleshooting

### Database Connection Errors

- Check that MongoDB is running or that your Atlas cluster is available.
- Verify the `MONGO_URI` value in `Backend/.env`.
- Confirm that your database user has the required permissions.

### Frontend Cannot Reach Backend

- Ensure the backend server is running.
- Verify the API base URL in the frontend configuration.
- Check browser developer tools for network or CORS errors.

### Packages Not Found

Run the following commands inside the affected application directory:

```bash
npm install
```

### Frontend Build Errors

```bash
npm run build
```

Review the terminal output and resolve any reported errors.

## Important Files

| File | Purpose |
|---|---|
| `Backend/server.js` | Backend application entry point |
| `Backend/package.json` | Backend dependencies and scripts |
| `Backend/config/db.js` | Database configuration |
| `Backend/models/` | Database models |
| `Backend/routes/` | API routes |
| `skillrise-web/package.json` | Frontend dependencies and scripts |
| `skillrise-web/src/App.jsx` | Main React application component |
| `skillrise-web/vite.config.js` | Vite configuration |
| `.gitignore` | Excludes files from Git tracking |

## Future Improvements

Potential improvements may include enhanced learning recommendations, additional career-planning features, improved analytics, and expanded user progress reporting.

## Author

**Tayyab Sajjad**

## Repository

[SkillRise on GitHub](https://github.com/tayyabsajjad76/SkillRise)

---

*SkillRise - Learning and Career Development Platform*