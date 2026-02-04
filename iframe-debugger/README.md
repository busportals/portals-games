# Iframe Debugger

A retro-styled terminal interface for debugging and testing iframe messages in Portals games.

## Features

- Classic green-on-black terminal aesthetic with CRT scan lines
- Displays messages with timestamps
- Auto-scrolls to latest message
- Close button (X) in top-right corner
- Listens for messages via PortalsSdk

## Usage

### Hosted URL
```
https://[your-github-pages-url]/iframe-debugger/
```

### Sending Messages

Use the `sendIframeMessage` function effect in Portals to send messages to the debugger:

```javascript
sendIframeMessage("Test message from trigger")
```

### Methods Used

- `PortalsSdk.setMessageListener()` - Receives messages from the game
- `PortalsSdk.closeIframe()` - Closes the iframe when X is clicked
- `PortalsSdk.focusGameKeyboard()` - Returns keyboard focus to the game

## Styling

The terminal features:
- Green (#0f0) monospace text
- Grey (>>>>) prompts
- White timestamps in ISO format
- Subtle CRT scan line effect
- Hidden scrollbar
