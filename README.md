# Personal Task Manager

A minimal personal task manager that runs entirely in your browser. No setup, no accounts—just open the HTML file and start tracking your tasks.

## How It Works

### Quick Wins
Short-term tasks with deadlines. Add a task, set a due date, check it off when done.

### Parking Lot
When you add a long-term goal to the Parking Lot, **you're required to break it down into smaller, deadline-driven tasks**. These subtasks automatically appear in your Quick Wins.

This solves a common problem: big personal projects that sit forever because they have no deadline. By forcing you to decompose a goal into concrete, time-bound actions, you actually make progress instead of letting it linger.

## Customization

### Name
Click "Click to set your name" on first use, or click the ✎ icon anytime to change it.

### Greeting
Find the `updateGreeting()` function in the code and edit the greeting text:
```javascript
if (hour >= 5 && hour < 12) {
  greeting = 'Good Morning';
} else if (hour >= 12 && hour < 17) {
  greeting = 'Good Afternoon';
}
// Default: 'Good Evening'
```

### Subtitle Quote
Find this line in the code and change the text:
```javascript
document.getElementById('subtitle-text').textContent = '— Focus on what matters';
```

### Colors
Edit the CSS variables in the `:root` section:
```css
:root {
  --bg-primary: #0a0a0a;        /* Main background */
  --bg-secondary: #18181b;      /* Card backgrounds */
  --accent-warm: #d97706;       /* Accent color (orange) */
  --text-primary: #fafafa;      /* Main text */
  --text-muted: #a1a1aa;        /* Secondary text */
}
```

## Data Privacy

All data is stored in your browser's local storage. Nothing is sent anywhere. Your tasks stay on your device, completely private.
