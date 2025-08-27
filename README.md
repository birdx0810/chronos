# ⏰ Chronos

A minimal, embeddable cron-based timer app that rings at scheduled intervals. Perfect for time tracking, productivity monitoring, and embedding in Notion or other platforms. 

## Features

- **Live Clock Display**: Shows current time in HH:MM:SS format
- **Cron-based Scheduling**: Use cron expressions for flexible timing patterns
- **Audio Notifications**: 5-second beeping sequence when intervals trigger
- **Responsive Design**: Optimized for embedding with minimal size requirements
- **Single Toggle Button**: Start/Stop functionality with double-click reset
- **Clean Interface**: Minimalist design that fits anywhere

## Cron Expression Format

```
minute hour day month weekday
```

**Common Examples:**
- `*/15 * * * *` - Every 15 minutes
- `0 * * * *` - Every hour on the hour  
- `*/15 9-17 * * 1-5` - Every 15 minutes during work hours (9-5) on weekdays
- `30 9 * * *` - Every day at 9:30 AM

## Usage

1. Enter a cron expression in the input field
2. Click the "Start" button to begin monitoring
3. The app will beep according to your schedule
4. Click "Stop" to pause, or double-click to reset

## Embedding

### Notion
1. Host the HTML file on any web service (CodePen, JSFiddle, Netlify, etc.)
2. Use Notion's `/embed` block with your hosted URL

### Optimal Embed Dimensions
- **Minimum**: 320px × 280px
- **Recommended**: 350px × 300px

### HTML Embed Code
```html
<iframe 
  src="YOUR_HOSTED_URL" 
  width="320" 
  height="280" 
  frameborder="0"
  style="border-radius: 10px;">
</iframe>
```

## Technical Details

- **Pure HTML/CSS/JavaScript** - No dependencies
- **Web Audio API** - For notification sounds
- **Responsive Design** - Adapts to container size
- **Browser Storage**: Uses in-memory storage only (no localStorage)

## Browser Compatibility

Works in all modern browsers that support:
- Web Audio API
- CSS Grid/Flexbox
- ES6 JavaScript

## License

Open source - feel free to modify and use as needed.

(Written using Claude Sonnet 4.)