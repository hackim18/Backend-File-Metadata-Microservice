# File Metadata Microservice

This project is a File Metadata Microservice built with Node.js and Express. The application allows users to upload a file and receive metadata about the file, such as its name, type, and size.

## Live Demo

You can see a live demo of the application here: [File Metadata Microservice](https://file-metadata-microservice.freecodecamp.rocks)

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [API Endpoint](#api-endpoint)
- [License](#license)

## Installation

1. **Clone the repository**:

   ```sh
   git clone https://github.com/your-username/file-metadata-microservice.git
   cd file-metadata-microservice
   ```

2. **Install dependencies**:

   ```sh
   npm install
   ```

3. **Create a .env file** in the root of the project and add the following line:

   ```sh
   PORT=3000
   ```

4. **Start the server**:
   ```sh
   npm start
   ```

The application will be running on http://localhost:3000.

## Usage

To use the File Metadata Microservice, you can access the following endpoint:

### API Endpoint

File Upload and Metadata

- URL: /api/fileanalyse
- Method: POST
- Description: Upload a file to receive its metadata.
- Request Body: Multipart/form-data with the file field named upfile.
- Example: http://localhost:3000/api/fileanalyse
- Response:
  ```json
  {
    "name": "filename.jpg",
    "type": "image/jpeg",
    "size": 1024
  }
  ```

## License

This project is licensed under the MIT License. See the LICENSE file for details.
