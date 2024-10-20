**Frontend-Trendle**
====================

Frontend of the **Trendle** project – a modern authentication system with login and signup functionalities integrated using **Firebase Authentication**. This project serves as the client-side interface to facilitate user access and registration.

* * *

**Table of Contents**
---------------------

*   [Installation](#installation)
*   [Features](#features)
*   [Technologies Used](#technologies-used)
*   [Getting Started](#getting-started)
*   [Authors](#authors)
*   [License](#license)

* * *

**Installation**
----------------

### Prerequisites

Ensure you have the following installed:

*   **Node.js** (Download from [https://nodejs.org](https://nodejs.org))
*   **Git** for version control (Download from [https://git\-scm.com](https://git-scm.com))

### Clone the Repository

```bash
git clone https://github.com/rushionsdomain/Frontend-Trendle-.git
cd Frontend-Trendle-
```

### Install Dependencies

Navigate to the project directory and install the required dependencies:

```bash
npm install
```

### Firebase Configuration

1.  Create a **Firebase project** at Firebase Console.
2.  Enable **Authentication** and add a new **web app** to get your Firebase configuration.
3.  Replace the content in `firebaseConfig.js` (inside the `src` folder) with your Firebase configuration:

```javascript
// firebaseConfig.js
import { initializeApp } from "firebase/app";
import { getAuth } from "firebase/auth";

const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_PROJECT_ID.firebaseapp.com",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_PROJECT_ID.appspot.com",
  messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
  appId: "YOUR_APP_ID",
};

const app = initializeApp(firebaseConfig);
export const auth = getAuth(app);
```

* * *

**Features**
------------

*   **User Authentication**: Login and Signup functionality using Firebase Authentication.
*   **Error Handling**: Displays error messages for invalid login or signup attempts.
*   **User Interface**: Simple and responsive UI with a bold title "Trendle".

* * *

**Technologies Used**
---------------------

*   **React.js**: Frontend framework for building the user interface.
*   **Firebase Authentication**: User authentication service for login/signup.
*   **CSS**: Styling the components for a responsive layout.
*   **Git & GitHub**: Version control and collaboration.

* * *

**Getting Started**
-------------------

### Start the Development Server

To run the project locally:

```bash
npm start
```

Open http://localhost:3000 in your browser to see the application.

* * *

**Authors**
-----------

**Frontend Authors:**

*   [Ahmed](#) – [GitHub Profile](https://github.com/Ahmed-824)
*   [Mercy](#) – [GitHub Profile](https://github.com/mercyhacker)
*   [Rushion](https://github.com/rushionsdomain) – [GitHub Profile](https://github.com/rushionsdomain)

Replace the `(#)` placeholders with the actual links to their GitHub profiles when available.

* * *

**License**
-----------

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

* * *

**Contributing**
----------------

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

* * *

**Deployment**
--------------

You can deploy this application to Firebase Hosting by running:

```bash
firebase deploy
```
