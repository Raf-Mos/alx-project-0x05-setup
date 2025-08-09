# ALX Project 0x05 Setup - Next.js Image Generation App

A comprehensive Next.js-based web application that allows users to generate AI-powered images by providing text prompts. This project demonstrates progressive development through multiple iterations, showcasing React best practices, state management, custom hooks, and API integration.

## 🎯 Project Overview

This project is a Next.js-based web application that interfaces with the GPT-4 Image Generation API to create unique images based on user input. The application features a clean UI with state management, custom hooks, and API integration, while following React best practices.

## 📚 Learning Objectives

By completing this project, you will:

- ✅ Understand and implement React state management using useState
- ✅ Create and utilize custom React hooks
- ✅ Work with environment variables for API key management
- ✅ Implement API routes in Next.js applications
- ✅ Develop reusable React components
- ✅ Manage application state across multiple components
- ✅ Implement responsive UI design with Tailwind CSS
- ✅ Handle asynchronous operations in React
- ✅ Follow React best practices for component structure and organization

## 🛠️ Requirements

- Node.js (v14 or later)
- Next.js (v13 or later)
- React (v18 or later)
- TypeScript
- Tailwind CSS
- GPT-4 API key (from RapidAPI)
- Modern web browser

## 📁 Project Structure

The project evolves through multiple versions (0x07 to 0x13), each adding new functionality:

```
alx-project-0x13/ (Final version)
├── components/
│   ├── common/
│   │   └── ImageCard.tsx          # Reusable image display component
│   └── layouts/
│       ├── Footer.tsx             # Application footer
│       ├── Header.tsx             # Application header with navigation
│       └── Layout.tsx             # Main layout wrapper
├── constants/
│   └── index.ts                   # Application constants (WIDTH, HEIGHT)
├── hooks/
│   └── useFetchData.ts           # Custom hook for API calls
├── interfaces/
│   └── index.ts                  # TypeScript interfaces and types
├── pages/
│   ├── api/
│   │   └── generate-image.ts     # API route for image generation
│   ├── _app.tsx                  # Next.js app component
│   └── index.tsx                 # Home page component
├── public/                       # Static assets
├── styles/
│   └── globals.css              # Global styles with Tailwind
├── .env.local                   # Environment variables (API keys)
├── .gitignore                   # Git ignore rules
├── next.config.js               # Next.js configuration
├── package.json                 # Dependencies and scripts
├── postcss.config.js            # PostCSS configuration
├── tailwind.config.js           # Tailwind CSS configuration
└── tsconfig.json                # TypeScript configuration
```

## 🚀 Quick Start

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/alx-project-0x05-setup.git
cd alx-project-0x05-setup
```

### 2. Choose Your Project Version

Navigate to any of the project versions:

```bash
# Basic setup (Task 0)
cd alx-project-0x07

# State management (Task 1)
cd alx-project-0x08

# Environment setup (Task 2)
cd alx-project-0x09

# API integration (Task 3)
cd alx-project-0x10

# Image tracking (Task 4)
cd alx-project-0x11

# Custom hooks (Task 5)
cd alx-project-0x12  # or alx-project-0x13
```

### 3. Install Dependencies

```bash
npm install
```

### 4. Set Up Environment Variables

Create a `.env.local` file in the project root:

```bash
NEXT_PUBLIC_GPT_API_KEY="your_rapidapi_key_here"
```

**To get your API key:**
1. Visit [RapidAPI](https://rapidapi.com/)
2. Sign up or log in
3. Search for "ChatGPT-42" API
4. Subscribe and get your API key

### 5. Run the Development Server

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

## 📋 Project Versions & Tasks

### Task 0: Basic Setup (alx-project-0x07)
**Objective:** Create the foundational Next.js application with basic layout components.

**Features:**
- Next.js project setup with TypeScript
- Header and Footer components
- Layout wrapper component
- Basic routing structure
- Tailwind CSS integration

### Task 1: State Management (alx-project-0x08)
**Objective:** Implement React state management and create reusable components.

**Features:**
- useState hooks for state management
- ImageCard component for displaying images
- Enhanced TypeScript interfaces
- State tracking for user inputs

### Task 2: Environment Setup (alx-project-0x09)
**Objective:** Configure environment variables for secure API key management.

**Features:**
- `.env.local` file configuration
- Environment variable access
- Security best practices

### Task 3: API Integration (alx-project-0x10)
**Objective:** Implement GPT-4 Image Generation API integration.

**Features:**
- API route for image generation
- External API calls to RapidAPI
- Constants for image dimensions
- Error handling and response processing

### Task 4: Image Tracking (alx-project-0x11)
**Objective:** Track and display generated images in a gallery format.

**Features:**
- Image history tracking
- Responsive image gallery
- Click-to-view functionality
- Enhanced state management

### Task 5: Custom Hooks (alx-project-0x12 & 0x13)
**Objective:** Create reusable custom hooks for better code organization.

**Features:**
- `useFetchData` custom hook
- Generic typing for reusability
- Cleaner component code
- Better separation of concerns

## 🔧 Key Features

### 🖼️ Image Generation
- Text prompt input
- AI-powered image generation via GPT-4
- Loading states during generation
- Real-time feedback

### 🖥️ User Interface
- Responsive design (mobile & desktop)
- Clean, modern interface
- Intuitive navigation
- Loading indicators

### 📱 Image Gallery
- History of generated images
- Thumbnail previews
- Click to view full image
- Responsive grid layout

### 🔒 Security
- API keys stored in environment variables
- Server-side API calls
- Input sanitization

### ⚡ Performance
- Custom hooks for reusable logic
- Optimized component structure
- Type-safe development

## 🏗️ Best Practices Implemented

### Component Organization
- Logical separation of layout and functional components
- Reusable components (ImageCard, Layout)
- Proper component typing with TypeScript

### State Management
- Proper use of React hooks (useState, useEffect)
- Custom hook for API calls (useFetchData)
- Type-safe state definitions

### API Handling
- Server-side API route for secure API key usage
- Proper error handling
- Loading states

### Type Safety
- TypeScript interfaces for all components and props
- Type-safe API responses
- Generic typing in custom hooks

## 📚 API Documentation

### Image Generation Endpoint

**Endpoint:** `POST /api/generate-image`

**Request Body:**
```json
{
  "prompt": "A beautiful sunset over mountains"
}
```

**Response:**
```json
{
  "message": "https://generated-image-url.com/image.jpg"
}
```

**Error Response:**
```json
{
  "error": "API key or URL is missing in environment variables"
}
```

## 🧪 Testing

### Manual Testing
1. Enter a text prompt in the input field
2. Click "Generate Image" button
3. Verify loading state appears
4. Check if image is generated and displayed
5. Test image gallery functionality

### Browser Console
- Open Developer Tools (F12)
- Check console for any errors
- Monitor network requests

## 🚀 Deployment

### Vercel (Recommended)

1. Push your code to GitHub
2. Connect your repository to [Vercel](https://vercel.com)
3. Add environment variables in Vercel dashboard
4. Deploy automatically

### Environment Variables for Production

```bash
NEXT_PUBLIC_GPT_API_KEY=your_production_api_key
```

## 📝 Development Notes

### Progressive Development
The project demonstrates progressive development through multiple versions:
- **0x07:** Basic setup and layout
- **0x08:** State management
- **0x09:** Environment configuration
- **0x10:** API integration
- **0x11:** Image tracking
- **0x12-0x13:** Custom hooks

### Code Quality
- Clean separation of concerns
- Reusable components and hooks
- Proper TypeScript implementation
- Good React patterns

## 🔮 Future Enhancements

For production use, consider adding:
- User authentication
- Persistent storage of generated images
- More advanced error handling
- Image editing capabilities
- Social sharing features
- Image download functionality
- Prompt suggestions
- Image filtering and search

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [ALX Software Engineering Program](https://www.alxafrica.com/)
- [Next.js Documentation](https://nextjs.org/docs)
- [React Documentation](https://reactjs.org/docs)
- [Tailwind CSS](https://tailwindcss.com/)
- [RapidAPI](https://rapidapi.com/)



