# Project Name: PickMe

## Description

PickMe is a next-generation minimalist social network designed for users who value authenticity, simplicity, and control over their privacy. Inspired by the formats of Threads and the philosophy of BeReal, PickMe addresses their key shortcomings:

- No forced random posting — users publish content whenever they choose.
- Full audience control — users explicitly select who sees each post: "Family", "Friends", "Everyone", or "Only Me".
- Maximum simplicity — a clean, uncluttered interface focused on content and meaningful interaction.
- Enhanced security — proactive measures against bots, fake accounts, and engagement manipulation.

PickMe is not just a feed; it is a private space for sharing genuine moments.

## Installation

The project is split into three independent repositories. To run a local version, each component must be set up separately.

### 1. Running the Backend API
```bash
# Clone the repository
git clone https://github.com/fpmi-hci-2025/project11b-backend-pickme.git
cd project11b-backend-pickme

# Run with Docker (recommended)
docker-compose up -d

# API will be available at: http://localhost:8000
# API documentation: http://localhost:8000/api/docs/
```

### 2. Running the Web Client
```bash
# Clone the repository
git clone https://github.com/fpmi-hci-2025/project11b-web-pickme.git
cd project11b-web-pickme

# Install dependencies
npm install

# Configure the environment file
cp .env.example .env
# Set: VITE_API_URL=http://localhost:8000

# Start the development server
npm run dev

# The application will be available at: http://localhost:3000
```

### 3. Running the Mobile Client (In Development)
The mobile application is currently under active development. Launch instructions will be added in a future update.

## Sub modules

This repository serves as a meta-repository (monorepo) that unifies all system components:

- **[Server & API Repository](https://github.com/fpmi-hci-2025/project11b-backend-pickme)**  
  A Python/Django backend providing REST API, authentication, post management, audience groups, and media handling.

- **[Web Client Repository](https://github.com/fpmi-hci-2025/project11b-web-pickme)**  
  A responsive web interface built with React and Tailwind CSS, focused on simplicity and user experience.

- **[Mobile Client Repository](https0://github.com/fpmi-hci-2025/project11b-mobile-pickme)**  
  A mobile application (in development) to be built using modern cross-platform technologies.

## Usage

After a successful launch:

1. Open the web application at `http://localhost:3000`.
2. Register with your email and a password.
3. Complete your profile and upload an avatar.
4. Navigate to the "Audience Groups" section and create your custom groups (e.g., "Family", "University").
5. Click the "+" button, write a note, attach photo/video/link, and explicitly select the audience.
6. Publish and enjoy a secure and controlled social experience.

### Key User Scenarios
- **For active users:** Publishing content with granular privacy settings and viewing basic statistics.
- **For passive users:** Safely browsing the feed without spam or intrusive notifications.

## Contributing

This project was developed by the following team members:

- [Yulia Kanoplich](https://github.com/Juliet165) — Business Analyst, UX Designer, Project Manager

- [Victoria Samsonova](https://github.com/victoriaSamsonovaaa) — System Analyst and Architect, UI Designer

- [Demid Moshkovich](https://github.com/IronGunYT) — Full Stack Developer
