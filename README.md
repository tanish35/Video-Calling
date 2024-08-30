## Overview

This is a fully functional video calling application built using modern web technologies. The app allows users to create and join video conferencing rooms where multiple participants can communicate in real-time. The app leverages Clerk.js for secure user authentication, Stream SDK for WebRTC connections, and is built with Next.js for a seamless user experience.

## Features

- **User Authentication:** Powered by Clerk.js, ensuring secure and easy login and registration for users.
- **Video Conferencing:** Create and join video rooms with multiple participants.
- **Real-Time Communication:** Utilizes Stream SDK to establish WebRTC connections for real-time video and audio communication between users.
- **Scalable Architecture:** Built on Next.js, offering server-side rendering, optimized performance, and a scalable foundation.

## Technology Stack

- **Next.js:** Framework for building the application with server-side rendering and static site generation.
- **Clerk.js:** Handles user authentication and management, providing a secure and user-friendly experience.
- **Stream SDK:** Provides WebRTC support for real-time video and audio communication.

## Getting Started

### Prerequisites

Before you start, make sure you have the following installed:

- Node.js
- npm or yarn
- A Clerk.js account
- A Stream SDK account

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/tanish35/Video-Calling.git
   cd video-calling-app
   ```

2. **Install dependencies:**
   ```bash
   npm install
   # or
   yarn install
   ```

### Set up environment variables:

Create a `.env.local` file in the root directory and add the following:

```bash
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=<your-clerk-publishable-key>
CLERK_SECRET_KEY=<your-clerk-secret-key>

NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up

NEXT_PUBLIC_STREAM_API_KEY=<your-stream-api-key>
STREAM_SECRET_KEY=<your-stream-secret-key>
```

Replace `<your-clerk-publishable-key>`, `<your-clerk-secret-key>`, `<your-stream-api-key>`, and `<your-stream-secret-key>` with your actual keys.

4. **Run the application:**
   ```bash
   npm run dev
   # or
   yarn dev
   ```

   Your app should now be running on [http://localhost:3000](http://localhost:3000).

## Usage

1. **Sign Up/Sign In:**
   Users can sign up or sign in using the Clerk.js authentication form.

2. **Create a Room:**
   Once authenticated, users can create a new video conference room.

3. **Join a Room:**
   Users can join an existing room by entering the room ID or following a shared link.

4. **Real-Time Communication:**
   After joining a room, users will be connected via Stream SDK’s WebRTC service, enabling real-time video and audio communication.

## Deployment

The app is already live and hosted at [vortex.devpixel.site](https://vortex.devpixel.site). 

For further development or deployment:

1. **Deploy to Vercel:**
   ```bash
   vercel
   ```

2. **Set environment variables in Vercel:**
   Make sure to add the same environment variables from your `.env.local` file to the Vercel dashboard.

3. **Access your deployed app:**
   Your app will be live at the domain provided by Vercel or another chosen hosting service.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request or open an issue if you have any suggestions or improvements.

## License

This project is licensed under the MIT License.

---

Feel free to reach out with any questions or feedback. Happy coding!
