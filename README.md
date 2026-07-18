Journey Through Romans
An interactive, single-page web application designed to help users study, review, and memorize the biblical Book of Romans (Chapters 1–16). Combining concise structural summaries, diagnostic quizzes, verse-reconstruction puzzles, and chronological sorting challenges, the application acts as a structured learning tool.
Features
1. Interactive Chapter Navigation
Sequential Progression: Chapter access is gated. Users earn tokens to unlock subsequent chapters.
Persistent Progress: Saves and loads your state automatically utilizing the browser's localStorage.
2. Four-Stage Learning Loop
📖 The Message: A brief synthesis of the chapter's theological focus, historical context, and a featured key memory verse.
❓ Knowledge Check (Quiz): Multiple-choice questions designed to test comprehension of major themes and details.
✍️ Verse Master (Fill in the Blank): Interactive word selection to reconstruct and memorize key verses.
⏳ Timeline (Order Events): A click-to-swap interface to sort narrative or theological developments into their original sequence.
3. Gamification and Feedback
Token System: Earn up to 30 tokens per chapter by demonstrating mastery across challenges.
Visual Progress Trackers: Track chapter-by-chapter and overall completion states in real-time.
Modern Responsive Dark Theme: Styled using CSS variables and flexbox/grid mechanics for readability across mobile and desktop displays.
Technical Overview
Language: Vanilla HTML5, CSS3, and JavaScript (ES6).
Dependencies: None. The application operates entirely client-side.
State Management: Driven by lightweight JavaScript state objects synchronized with native localStorage.
How to Run the Project Locally
Because this application relies on standard web technologies with no build steps, running it is straightforward:
Clone or download this repository.
code
Bash
git clone https://github.com/your-username/journey-through-romans.git
Navigate to the directory containing the project file.
Double-click JourneyThroughRomans.html to open it in any modern web browser (such as Chrome, Firefox, Safari, or Edge).
How to Deploy on GitHub Pages
You can easily host this application for free using GitHub Pages:
Push your files to a GitHub repository.
In your repository on GitHub, navigate to Settings > Pages (under the "Code and automation" sidebar menu).
Under Build and deployment, set the Source to Deploy from a branch.
Select the branch (usually main or master) and folder (usually /root) containing JourneyThroughRomans.html (Note: You may want to rename your file to index.html to make it the default landing page).
Click Save. Within a few minutes, your site will be live at [https://2ndchances520.github.io/JourneyThroughRomans/].
Data Structure
The application's content is managed via a JSON-like array inside the script block, allowing for easy expansion, content corrections, or local translation efforts.
code
JavaScript
{
    num: 1,
    title: "Introduction",
    summary: "Paul introduces the power of the Gospel...",
    verse: "For I am not ashamed...",
    ref: "Romans 1:16",
    questions: [
        { q: "Who wrote Romans?", a: ["Peter","Paul","John","Luke"], c: 1 }
    ],
    fill: {
        text: "I am not ____ of the ____ of Christ.",
        words: ["ashamed", "gospel"],
        options: ["ashamed", "afraid", "gospel", "message"]
    },
    order: [
        "Paul identifies as a servant",
        "He declares his mission",
        "The theme of faith is set"
    ]
}
License
This project is open-source and available under the MIT License.
