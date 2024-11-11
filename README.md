# StoreIt - It's a cloud vault. YOUR cloud vault.

## 🌟 Overview
StoreIt is a modern cloud storage solution built with Next.js 14, offering a secure and intuitive way to store and manage digital files. This project was created following the tutorial by [JavaScript Mastery](https://www.youtube.com/watch?v=lie0cr3wESQ).

![StoreIt Banner](https://i.ibb.co/wR9G2k3/Readme-Thumbnail.png)

<div>
     <img src="https://img.shields.io/badge/-Next_JS-black?style=for-the-badge&logoColor=white&logo=nextdotjs&color=000000" alt="nextdotjs" />
    <img src="https://img.shields.io/badge/-TypeScript-black?style=for-the-badge&logoColor=white&logo=typescript&color=3178C6" alt="typescript" />
    <img src="https://img.shields.io/badge/-Tailwind_CSS-black?style=for-the-badge&logoColor=white&logo=tailwindcss&color=06B6D4" alt="tailwindcss" />
    <img src="https://img.shields.io/badge/-Appwrite-black?style=for-the-badge&logoColor=white&logo=appwrite&color=FD366E" alt="appwrite" />
  </div>

## ⚡ Key Features
- 📁 File Management (Upload, Download, Share)
- 🔍 Advanced Search Capabilities
- 📊 Storage Analytics & Visualization
- 🎯 File Type Categorization
- 🔐 Secure Authentication
- 📱 Responsive Design
- 💫 Modern UI/UX
- 🚀 Real-time Updates

## 🛠️ Tech Stack
- **Framework**: Next.js 14
- **Styling**: Tailwind CSS
- **Authentication**: Appwrite
- **File Storage**: Appwrite Storage
- **UI Components**: Shadcn/ui
- **Charts**: Recharts
- **State Management**: React Hooks
- **Icons**: Custom SVG Icons

## 📋 Prerequisites
Before you begin, ensure you have:
- Node.js 18+ installed
- Appwrite account and server setup
- npm or yarn package manager

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/storeit.git
cd storeit
```

### 2. Install Dependencies

### 3. Environment Setup
Create a `.env.local` file in the root directory:
```env
NEXT_PUBLIC_APPWRITE_PROJECT_ID=your_project_id
NEXT_PUBLIC_APPWRITE_ENDPOINT=your_endpoint
NEXT_PUBLIC_APPWRITE_STORAGE_ID=your_storage_id
NEXT_PUBLIC_APPWRITE_DATABASE_ID=your_database_id
```

### 4. Appwrite Setup
1. Create a new project in Appwrite Console
2. Create a new database
3. Set up storage bucket
4. Configure authentication methods
5. Update security settings and CORS

### 5. Run Development Server
```bash
npm run dev
# or
yarn dev
```

## 📁 Project Structure
```
storeit/
├── app/
│   ├── (auth)/
│   │   ├── sign-in/
│   │   └── sign-up/
│   ├── (root)/
│   │   ├── [type]/
│   │   └── page.tsx
│   └── layout.tsx
├── components/
├── constants/
├── lib/
│   ├── actions/
│   └── utils/
├── public/
│   ├── assets/
│   └── fonts/
└── types/
```

## 🎯 Core Features Explained

### Authentication
- Secure sign-up and sign-in
- OAuth integration
- Session management

### File Management
- Multi-file upload support
- Progress tracking
- File type validation
- Secure sharing mechanisms

### Dashboard Analytics
- Storage usage visualization
- File type distribution
- Upload history
- Space management

### Search Functionality
- Real-time search
- File type filtering
- Advanced sorting options

## 🔧 Configuration Options

### Customizing File Types
```typescript
// constants/index.ts
export const allowedFileTypes = {
  documents: ['pdf', 'doc', 'docx', 'txt'],
  images: ['png', 'jpg', 'jpeg', 'gif'],
  media: ['mp4', 'mp3', 'wav'],
  others: ['zip', 'rar']
};
```

### Storage Limits
```typescript
export const STORAGE_LIMITS = {
  free: 5 * 1024 * 1024 * 1024, // 5GB
  premium: 50 * 1024 * 1024 * 1024 // 50GB
};
```

## 🎨 Styling Customization
The project uses Tailwind CSS with custom configuration:
```typescript
// tailwind.config.js
module.exports = {
  theme: {
    extend: {
      colors: {
        brand: {...},
        dark: {...},
        light: {...}
      }
    }
  }
};
```

## 📱 Responsive Design
- Mobile-first approach
- Breakpoints:
  - sm: 640px
  - md: 768px
  - lg: 1024px
  - xl: 1280px

## ⚡ Performance Optimizations
- Image optimization
- Lazy loading
- Code splitting
- API response caching
- Static site generation where applicable

## 🔐 Security Features
- Encrypted file storage
- Secure file sharing
- Authentication tokens
- Rate limiting
- Input sanitization

## 🧪 Testing
```bash
# Run tests
npm run test

# Run tests with coverage
npm run test:coverage
```

## 📦 Deployment
1. Build the project:
```bash
npm run build
```

2. Start production server:
```bash
npm start
```

## 🤝 Contributing
1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Open a pull request

## 📄 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments
- [JavaScript Mastery](https://www.youtube.com/@javascriptmastery) for the excellent tutorial and frontend assets
- [Appwrite](https://appwrite.io/) for backend services
- [Shadcn/ui](https://ui.shadcn.com/) for UI components
- [Tailwind CSS](https://tailwindcss.com/) for styling

## 🔄 Updates
Stay tuned for updates:
- [ ] Team collaboration features
- [ ] Advanced file preview
- [ ] Mobile apps
- [ ] API access

Created with 💙 by Pakagrong Lebel
