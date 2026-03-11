# Chat Bot

A feature-rich chat bot application built with vanilla HTML, CSS, and JavaScript. No frameworks, no build tools, no API keys required (except for weather which uses a free public API).

## Features

### Pattern-Based Chat

The bot responds to messages using keyword pattern matching. Supported topics include greetings, jokes, time/date, and general conversation with randomized replies for a natural feel.

### Live Weather Search

Get real-time weather data for any city worldwide powered by the [Open-Meteo API](https://open-meteo.com/) (free, no API key needed). Returns current temperature, weather condition, humidity, and wind speed.

**Usage:**

- Type `weather in Tokyo` in the chat
- Or click the **Weather** quick-action button and enter a city name

### Flight Search

Search for flights between any two cities. Returns 3 flight options with randomized airlines, departure/arrival times, duration, and pricing (mock data).

**Usage:**

- Type `flights from London to Paris` in the chat
- Or click the **Flights** quick-action button and fill in the From/To fields

### Conversation Memory

The bot remembers facts you share about yourself and persists them across browser sessions using `localStorage`.

**What it remembers:**

- Name: `My name is Shyma`
- Location: `I live in Dubai`
- Age: `I'm 25 years old`
- Job: `I work as a developer at Google`
- Favorites: `My favorite color is blue`
- Likes: `I love coding`

**Recall commands:**

- `What do you remember about me` - shows everything stored
- `What's my name` / `What's my job` - recalls specific info
- `Forget my memory` - clears all stored data

The bot also personalizes greetings with your name and displays a welcome-back message on return visits.

### Voice Input (Speech to Text)

Click the microphone button to speak your message instead of typing. Uses the browser's built-in Web Speech API.

- Real-time transcription as you speak
- Auto-sends the message when you stop talking
- Pulsing red indicator while recording
- Click again to cancel mid-recording
- Graceful handling for denied permissions or unsupported browsers

### Quick Action Buttons

Dedicated **Weather** and **Flights** buttons provide inline forms for fast access without needing to type the full command.

## Getting Started

1. Clone or download the project
2. Open `index.html` in a modern browser (Chrome, Edge, or Safari recommended)

```bash
open index.html
```

No installation, no dependencies, no build step.

## Tech Stack

- **HTML5** - Structure
- **CSS3** - Styling with flexbox layout, animations
- **Vanilla JavaScript** - All logic, no frameworks
- **Open-Meteo API** - Free weather data (no API key)
- **Web Speech API** - Browser-native speech recognition
- **localStorage** - Client-side memory persistence

## Browser Support

| Feature             | Chrome | Edge | Safari | Firefox |
| ------------------- | ------ | ---- | ------ | ------- |
| Chat                | Yes    | Yes  | Yes    | Yes     |
| Weather API         | Yes    | Yes  | Yes    | Yes     |
| Flight Search       | Yes    | Yes  | Yes    | Yes     |
| Conversation Memory | Yes    | Yes  | Yes    | Yes     |
| Voice Input         | Yes    | Yes  | Yes    | No      |

> Voice input requires the Web Speech API, which is not supported in Firefox.

## Project Structure

```
chat-bot/
  index.html   # Single-file application (HTML + CSS + JS)
  README.md    # This file
```

## License

MIT
