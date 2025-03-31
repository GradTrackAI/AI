# College Admissions Advisor

A comprehensive AI-powered college admissions guidance platform that leverages advanced machine learning to provide personalized insights for student application strategies.

## Features

- **Multi-step Form**: Easy-to-use interface to collect student profile information
- **Personalized Analysis**: AI-powered evaluation of college admission chances
- **Detailed Recommendations**: Customized improvement plans for each student
- **College Matching**: Analysis of fit with specific colleges and majors
- **User Accounts**: Save and review past assessments (requires authentication)

## Technologies Used

- **Frontend**: React.js with TypeScript
- **Styling**: Tailwind CSS
- **Authentication**: Supabase Authentication
- **API Integration**: DeepSeek AI for admissions analysis
- **State Management**: React Query and Context API

## Running the Application

### Full Application (with Backend)

The complete application provides all features including user authentication, saving results, and AI-powered analysis.

1. Clone the repository
2. Install dependencies:
   ```
   npm install
   ```
3. Set up environment variables:
   - Create a `.env` file in the root directory
   - Add the following variables:
     ```
     SUPABASE_URL=your_supabase_url
     SUPABASE_ANON_KEY=your_supabase_anon_key
     DEEPSEEK_API_KEY=your_deepseek_api_key
     EMAIL_USER=your_email_user (optional for email verification)
     EMAIL_PASSWORD=your_email_password (optional for email verification)
     ```
4. Start the application:
   ```
   npm run dev
   ```
5. Open your browser and navigate to `http://localhost:5000`

### Static Demo Version (No Backend Required)

A simplified version is available for demo purposes. This version has all the UI elements without requiring a server or API keys.

1. Navigate to the `/static-version` directory
2. Open `index.html` in any web browser
3. Interact with the form to see a pre-configured example analysis

## Project Structure

- `/client`: React frontend application
  - `/src/components`: UI components
  - `/src/hooks`: Custom React hooks
  - `/src/lib`: Utility functions and API clients
  - `/src/pages`: Application pages
- `/server`: Express backend server
  - `routes.ts`: API endpoints
  - `storage.ts`: Data storage interface
  - `index.ts`: Server configuration
- `/shared`: Shared TypeScript types and schemas
- `/static-version`: Standalone HTML demo version

## Deployment

The application can be deployed to:

1. **GitHub Pages**: Deploy the static version for demonstration
2. **Replit**: Deploy the full application with backend support
3. **Vercel/Netlify**: Deploy the frontend with serverless functions

## Developing

1. Create a new feature branch
2. Make your changes
3. Run tests (if available)
4. Submit a pull request

## License

[MIT License](LICENSE)

## Acknowledgements

- DeepSeek AI for providing the analysis capabilities
- Supabase for authentication services
- Tailwind and Shadcn UI for styling components