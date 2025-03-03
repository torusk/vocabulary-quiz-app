# Vocabulary Quiz App

This is a simple vocabulary quiz application built with Next.js and React. It allows users to upload a JSON dataset of vocabulary questions and take a quiz based on that dataset.

## Project Structure

\`\`\`
vocabulary-quiz-app/
├── app/
│   └── page.tsx
├── components/
│   └── ui/
│       ├── button.tsx
│       ├── card.tsx
│       ├── label.tsx
│       └── radio-group.tsx
├── lib/
│   └── utils.ts
├── public/
├── README.md
└── package.json
\`\`\`

## Setup

1. Clone the repository:
   \`\`\`
   git clone https://github.com/your-username/vocabulary-quiz-app.git
   cd vocabulary-quiz-app
   \`\`\`

2. Install dependencies:
   \`\`\`
   npm install
   \`\`\`

## Running the Application

1. Start the development server:
   \`\`\`
   npm run dev
   \`\`\`

2. Open your browser and navigate to \`http://localhost:3000\`

## Using the Application

1. Prepare a JSON file with your vocabulary questions. The file should have the following structure:
   \`\`\`json
   {
     "vocabulary": [
       {
         "word": "example",
         "meaning": "a representative form or pattern",
         "example": "This is an example sentence.",
         "question": "What word means 'a representative form or pattern'?",
         "options": ["example", "sample", "model", "instance"]
       },
       // ... more questions ...
     ]
   }
   \`\`\`

2. When you open the application, you'll see an option to upload your JSON file.

3. After uploading, the quiz will start automatically.

4. For each question:
   - You have 5 seconds to answer
   - If you don't answer within 5 seconds, it will show the correct answer
   - After answering or after the time is up, you'll see an explanation with the correct answer, meaning, and an example sentence

5. At the end of the quiz, you'll see your score and have an option to restart the quiz.

Enjoy improving your vocabulary!

## Styling and Customization

This project uses Tailwind CSS for styling. The main styling is done inline in the `app/page.tsx` file. Here's how you can customize the appearance:

1. **Color Scheme**: The main color scheme is defined in the background of the main container. You can change it by modifying the `bg-gradient-to-r from-blue-500 to-purple-600` classes.

2. **Card Styling**: The quiz card uses the `Card` component from `@/components/ui/card`. You can customize its appearance by modifying the `Card`, `CardHeader`, `CardContent`, and `CardFooter` components in `components/ui/card.tsx`.

3. **Button Styling**: Buttons use the `Button` component from `@/components/ui/button`. Customize their appearance in `components/ui/button.tsx`.

4. **Typography**: Font sizes and styles are set using Tailwind classes like `text-2xl`, `font-bold`, etc. You can adjust these directly in `app/page.tsx`.

5. **Layout**: The layout of the quiz (grid for options, spacing, etc.) is controlled by Tailwind classes in `app/page.tsx`. Modify these to change the layout.

6. **Responsive Design**: The current design is responsive, but you can add more breakpoints or adjust the existing ones using Tailwind's responsive prefixes (sm:, md:, lg:, etc.) in `app/page.tsx`.

To make global style changes, you can edit the Tailwind configuration file (`tailwind.config.js`) to add custom colors, fonts, or modify existing theme values.

Remember to rebuild your application after making changes to see the updates.

