# AssaignmentFrontend

This project was generated using [Angular CLI](https://github.com/angular/angular-cli) version 20.0.1.

## Development server

To start a local development server, run:

```bash
ng serve
```

Once the server is running, open your browser and navigate to `http://localhost:4200/`. The application will automatically reload whenever you modify any of the source files.

## Code scaffolding

Angular CLI includes powerful code scaffolding tools. To generate a new component, run:

```bash
ng generate component component-name
```

For a complete list of available schematics (such as `components`, `directives`, or `pipes`), run:

```bash
ng generate --help
```

## Building

To build the project run:

```bash
ng build
```

This will compile your project and store the build artifacts in the `dist/` directory. By default, the production build optimizes your application for performance and speed.

## Running unit tests

To execute unit tests with the [Karma](https://karma-runner.github.io) test runner, use the following command:

```bash
ng test
```

## Running end-to-end tests

For end-to-end (e2e) testing, run:

```bash
ng e2e
```

Angular CLI does not come with an end-to-end testing framework by default. You can choose one that suits your needs.

## Additional Resources

For more information on using the Angular CLI, including detailed command references, visit the [Angular CLI Overview and Command Reference](https://angular.dev/tools/cli) page.










📝 Note Keeper Frontend
This is the frontend client for the Note Keeper Application, built using Angular. It interacts with a RESTful backend to manage notes with full CRUD operations (Create, Read, Update, Delete).

🔧 Tech Stack
Framework: Angular (v13+)

Styling: CSS3 (Optionally Tailwind/Bootstrap)

Communication: HTTPClient (REST API)

Forms: Template-driven or Reactive Forms

Icons/UI: Optional libraries like Angular Material or FontAwesome

⚙️ Features
Add new notes with title, description, and tag

Edit or delete existing notes

View all notes in a responsive layout

Connected to backend API via services

Clean and modular component structure

📦 Folder Structure
css
Copy
Edit
src/
├── app/
│   ├── components/
│   │   ├── note-form/
│   │   └── note-list/
│   ├── services/
│   │   └── note.service.ts
│   ├── models/
│   │   └── note.model.ts
│   ├── app.component.ts
│   └── app.module.ts
├── assets/
├── index.html
└── styles.css
🚀 Getting Started
Clone the repo

bash
Copy
Edit
git clone https://github.com/your-username/note-keeper-frontend.git
cd note-keeper-frontend
Install dependencies

bash
Copy
Edit
npm install
Run the app

bash
Copy
Edit
ng serve
Access it
Navigate to http://localhost:4200 in your browser.

🔗 Backend Integration
Make sure your backend server is running (see backend README) and update the API base URL in note.service.ts if necessary:

ts
Copy
Edit
private apiUrl = 'http://localhost:5000/api/notes';
You can also use environment variables (environment.ts) to manage URLs for dev/prod.

📡 API Usage (Handled in note.service.ts)
Method	Endpoint	Description
GET	/api/notes	Fetch all notes
POST	/api/notes	Create a new note
PUT	/api/notes/:id	Update a note
DELETE	/api/notes/:id	Delete a note

🖥️ Components Overview
Component	Purpose
note-form	Input form to add or edit notes
note-list	Displays list of notes with actions
app.component	Main shell combining the above

🧪 Testing
You can run unit tests using:

bash
Copy
Edit
ng test
