# Background Remover

## Overview

Background Remover is a project designed to automatically remove the background from any given image. The tool leverages advanced machine learning algorithms to identify and separate the foreground object from the background, producing a clean, isolated image of the subject.

## Features

- **Automatic Background Removal**: Uses deep learning models to accurately detect and remove backgrounds.
- **Supports Multiple Image Formats**: Works with JPEG, PNG, BMP, and more.
- **User-Friendly Interface**: Easy-to-use GUI for non-technical users.
- **API Support**: REST API for integration with other applications.

## Technology Stack

- **Frontend**: React.js
- **Backend**: Node.js, Express.js

## Installation

### Prerequisites

- Node.js and npm

### Steps

1. **Clone the repository**:

   ```bash
   git clone https://github.com/NaveKattan/Picture_BG.git
   cd Picture_BG
   ```

2. **Install frontend dependencies**:

   ```bash
   npm install
   ```

3. **Install backend dependencies**:

   ```bash
   cd backend
   npm install
   ```

4. **Run the application**:
   - **Frontend**:
     ```bash
     npm start
     ```
   - **Backend**:
     ```bash
     cd backend
     npm start
     ```

## Usage

1. **Upload an Image**: use the file upload button.
2. **Process the Image**: Click on the "Remove Background" button.
3. **Download the Result**: Once processing is complete, download the image with the background removed.

## API Endpoints

### POST /api/remove-background

Removes the background from an uploaded image.

- **Request**:

  - `image`: The image file to process

- **Response**:
  - `200 OK`: Returns the processed image
  - `400 Bad Request`: If the image is not provided or is in an unsupported format
