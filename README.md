# MediScan AI - Advanced Disease Detection System

A modern, AI-powered health analysis system built with Next.js, TypeScript, and Tailwind CSS. This application helps users identify potential medical conditions based on their symptoms and provides intelligent recommendations.

## 🚀 Features

- **Intelligent Symptom Analysis**: Advanced AI-powered diagnosis engine that combines multiple symptoms into comprehensive analysis
- **Mobile Swipe Interface**: Smooth horizontal swipe navigation between Health Assistant and Results on mobile devices
- **Combined Analysis**: Multiple symptoms are analyzed together to provide a single, comprehensive diagnosis instead of separate results
- **Modern UI/UX**: Professional, responsive design with smooth animations using Framer Motion
- **Comprehensive Database**: Extensive medical conditions database with detailed information
- **Smart Recommendations**: Personalized recommendations based on symptom severity and combination patterns
- **Real-time Analysis**: Instant analysis with visual feedback and loading states
- **Accessibility**: Built with accessibility best practices and WCAG guidelines
- **Responsive Layout**: Desktop side-by-side layout, mobile swipe interface with input card positioned below main content

## 🛠️ Technology Stack

- **Framework**: Next.js 15 with App Router
- **Language**: TypeScript
- **Styling**: Tailwind CSS
- **Animations**: Framer Motion
- **Icons**: Lucide React
- **UI Components**: Radix UI primitives
- **Font**: Inter (Google Fonts)

## 📋 Prerequisites

- Node.js 18.0 or later
- npm, yarn, or pnpm package manager

## 🚀 Getting Started

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd disease-detection-system
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
   # or
   pnpm install
   ```

3. **Run the development server**
   ```bash
   npm run dev
   # or
   yarn dev
   # or
   pnpm dev
   ```

4. **Open your browser**
   Navigate to [http://localhost:3000](http://localhost:3000) to see the application.

## 🏗️ Project Structure

```
src/
├── app/                    # Next.js App Router
│   ├── globals.css        # Global styles
│   ├── layout.tsx         # Root layout
│   └── page.tsx          # Home page
├── components/            # React components
│   ├── DiseaseDetectionSystem.tsx  # Main application component
│   ├── SymptomInput.tsx            # Symptom input interface
│   └── DiagnosisResults.tsx        # Results display component
├── lib/                   # Utility functions and logic
│   ├── diagnosisEngine.ts # AI diagnosis engine
│   └── utils.ts          # Common utilities
└── types/                # TypeScript type definitions
    └── diagnosis.ts      # Medical data types
```

## 🧠 How It Works

### Diagnosis Engine

The application uses an advanced symptom matching algorithm that:

1. **Normalizes Input**: Processes user symptoms and standardizes terminology
2. **Pattern Matching**: Uses both direct and fuzzy matching for symptom recognition
3. **Confidence Scoring**: Calculates confidence levels based on symptom matches and severity
4. **Risk Assessment**: Determines urgency levels for medical attention
5. **Recommendations**: Provides personalized care recommendations

### Key Features

- **Symptom Input**: Users can add symptoms manually or select from common conditions
- **Severity Tracking**: Each symptom can be rated as mild, moderate, or severe
- **Duration Logging**: Track how long symptoms have been present
- **Real-time Analysis**: Instant processing with visual feedback
- **Comprehensive Results**: Detailed analysis with match percentages and recommendations

## 🎨 UI Components

### Main Components

- **DiseaseDetectionSystem**: Main application wrapper with state management
- **SymptomInput**: Interactive symptom input interface with common symptoms
- **DiagnosisResults**: Professional results display with animations and urgency indicators

### Design Features

- **Gradient Backgrounds**: Modern gradient designs for visual appeal
- **Smooth Animations**: Framer Motion animations for enhanced UX
- **Professional Typography**: Inter font for clean, readable text
- **Color-coded Urgency**: Visual indicators for different urgency levels
- **Responsive Grid**: Adaptive layout for all screen sizes

## ⚠️ Medical Disclaimer

**IMPORTANT**: This application is designed for educational and informational purposes only. It should not replace professional medical advice, diagnosis, or treatment. Always consult with qualified healthcare professionals for medical concerns. In case of emergency, contact your local emergency services immediately.

## 🔧 Customization

### Adding New Medical Conditions

Edit `src/lib/diagnosisEngine.ts` and add new conditions to the `MEDICAL_CONDITIONS` array:

```typescript
{
  name: 'Condition Name',
  description: 'Detailed description',
  commonSymptoms: ['symptom1', 'symptom2'],
  severity: 'mild' | 'moderate' | 'severe',
  urgency: 'non-urgent' | 'routine' | 'urgent' | 'immediate',
  category: 'category_name',
  recommendations: ['recommendation1', 'recommendation2']
}
```

### Styling Customization

The application uses Tailwind CSS for styling. Customize colors, spacing, and components by:

1. Editing `tailwind.config.js` for theme customization
2. Modifying component classes in individual component files
3. Updating global styles in `src/app/globals.css`

## 📱 Responsive Design

The application is fully responsive and optimized for:

- **Desktop**: Full-featured interface with side-by-side layout
- **Tablet**: Adapted grid layout with touch-friendly controls
- **Mobile**: Stacked layout with optimized input methods

## 🚀 Deployment

### Vercel (Recommended)

1. Push your code to GitHub
2. Connect your repository to Vercel
3. Deploy with zero configuration

### Other Platforms

The application can be deployed to any platform that supports Next.js:

- Netlify
- AWS Amplify
- Railway
- Heroku

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🆘 Support

If you encounter any issues or have questions:

1. Check the existing issues on GitHub
2. Create a new issue with detailed information
3. Provide steps to reproduce any bugs

## 🙏 Acknowledgments

- Medical condition data compiled from various medical resources
- UI/UX inspiration from modern healthcare applications
- Icons provided by Lucide React
- Animations powered by Framer Motion