# J.A.T.E. (Just Another Text Editor)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub issues](https://img.shields.io/github/issues/ngojohn2002/jate)](https://github.com/ngojohn2002/jate/issues)
[![GitHub forks](https://img.shields.io/github/forks/ngojohn2002/jate)](https://github.com/ngojohn2002/jate/network)
[![GitHub stars](https://img.shields.io/github/stars/ngojohn2002/jate)](https://github.com/ngojohn2002/jate/stargazers)

J.A.T.E. is a Progressive Web Application (PWA) that allows you to create notes or code snippets with or without an internet connection. This application leverages modern web technologies to provide a seamless and robust text editing experience.

## Table of Contents

- [Features](#features)
- [User Story](#user-story)
- [Acceptance Criteria](#acceptance-criteria)
- [Demo](#demo)
- [Installation](#installation)
- [Usage](#usage)
- [Testing](#testing)
- [Built With](#built-with)
- [Contributing](#contributing)
- [Credits](#credits)
- [License](#license)

## Features

- **Offline Functionality**: Works offline and syncs data when reconnected to the internet.
- **Service Workers**: Uses service workers for caching and offline access.
- **IndexedDB**: Stores data in IndexedDB for persistent storage.
- **Responsive Design**: Optimized for various screen sizes.
- **PWA Installation**: Installable on desktops and mobile devices.

[Back to Table of Contents](#table-of-contents)

## User Story

```
AS A developer  
I WANT to create notes or code snippets with or without an internet connection  
SO THAT I can reliably retrieve them for later use
```

[Back to Table of Contents](#table-of-contents)

## Acceptance Criteria

- The application should be deployed on Render.
- The application should have a generated `manifest.json` using the `WebpackPwaManifest` plugin.
- The application should have a registered service worker using Workbox.
- The application should be installable as a PWA.
- IndexedDB should be used to create an object store and include both GET and PUT methods.
- The application should use a package like `idb` to handle IndexedDB logic.
- The editor should function offline and retrieve data from the IndexedDB when it is available.
- Content in the editor should be automatically saved when the editor loses focus.

[Back to Table of Contents](#table-of-contents)

## Demo

A live demo of the application can be accessed [here](http://your-demo-url.com).

[Back to Table of Contents](#table-of-contents)

## Installation

Follow these steps to set up the project locally.

### Prerequisites

- Node.js
- npm (Node Package Manager)

### Clone the Repository

```bash
git clone https://github.com/ngojohn2002/jate.git
cd jate
```

### Install Dependencies

#### Client-side

```bash
cd client
npm install
```

#### Server-side

```bash
cd ../server
npm install
```

[Back to Table of Contents](#table-of-contents)

## Usage

### Running in Development Mode

To start the development server and run the application locally:

```bash
cd client
npm run dev
```

Open your browser and navigate to `http://localhost:8080`.

### Building for Production

To create a production build of the application:

```bash
npm run build
```

### Starting the Server

To start the server and serve the production build:

```bash
cd ../server
npm run server
```

Open your browser and navigate to `http://localhost:3000`.

[Back to Table of Contents](#table-of-contents)

## Testing

### Verifying Offline Capabilities

1. **Open DevTools**:
   - Right-click on the application page and select "Inspect" or press `F12`.

2. **Simulate Offline Mode**:
   - Go to the "Network" tab in DevTools.
   - Select "Offline" from the throttling dropdown menu.

3. **Test Offline Functionality**:
   - Refresh the page to see if the application still works and serves cached content.
   - Navigate through different parts of the application to verify that all necessary assets are available offline.

### Running Lighthouse Audit

Lighthouse is an automated tool for improving the quality of web pages. To run a Lighthouse audit:

1. **Open DevTools**:
   - Go to the "Lighthouse" tab.
   
2. **Run Lighthouse Audit**:
   - Select the categories you want to audit (e.g., Performance, Progressive Web App, Best Practices).
   - Click "Generate report" to run the audit.

3. **Review the Report**:
   - Check the PWA section for compliance and suggestions.
   - Address any issues or warnings highlighted in the report.

[Back to Table of Contents](#table-of-contents)

## Built With

- **Node.js**: ![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
- **Express**: ![Express](https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white)
- **Webpack**: ![Webpack](https://img.shields.io/badge/Webpack-8DD6F9?style=for-the-badge&logo=webpack&logoColor=white)
- **Babel**: ![Babel](https://img.shields.io/badge/Babel-F9DC3E?style=for-the-badge&logo=babel&logoColor=white)
- **Workbox**: ![Workbox](https://img.shields.io/badge/Workbox-3D8DD6?style=for-the-badge&logo=workbox&logoColor=white)
- **IndexedDB**: ![IndexedDB](https://img.shields.io/badge/IndexedDB-4B0082?style=for-the-badge&logo=indexeddb&logoColor=white)

[Back to Table of Contents](#table-of-contents)

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create your feature branch (`git checkout -b feature/YourFeature`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a pull request.

[Back to Table of Contents](#table-of-contents)

## Credits

This project was made possible with the help of [ChatGPT](https://chatgpt.com/).

[Back to Table of Contents](#table-of-contents)

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

[Back to Table of Contents](#table-of-contents)

---

© 2024 Truong Ngo. All rights reserved.

(19 PWA - Progressive Web Application)
