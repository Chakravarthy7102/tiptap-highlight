# @devchaks/tiptap-highlight

A customizable highlight extension for the Tiptap editor.

## Additional Features Support

- Assigns unique IDs to highlighted text, enabling custom actions and improved text manipulation

## Installation

```bash
npm install @devchaks/tiptap-highlight
```

## Usage

```javascript
import { Editor } from "@tiptap/core";
import { Highlight } from "@devchaks/tiptap-highlight";

const editor = new Editor({
  extensions: [
    Highlight.configure({
      multicolor: true,
    }),
    // ... other extensions
  ],
});
```

## Configuration

The Highlight extension can be configured with the following options:

- `multicolor`: Boolean (default: `false`) - Enables multicolor highlighting
- `HTMLAttributes`: Object - Additional HTML attributes to be added to the highlight mark

## Commands

- `setHighlight(attributes)`: Apply highlight with optional color and id
- `toggleHighlight(attributes)`: Toggle highlight with optional color
- `unsetHighlight()`: Remove highlight

## Keyboard Shortcuts

- `Mod-Shift-h`: Toggle highlight (default)

## Input Rules

Automatically highlights text wrapped in double equals signs:

```
==highlighted text==
```

## Paste Rules

Preserves highlights when pasting text with the `==highlighted text==` format.

## API

### Highlight

```javascript
import { Highlight } from "@devchaks/tiptap-highlight";
```

#### Options

```javascript
Highlight.configure({
  multicolor: true,
  HTMLAttributes: {},
});
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License.

## Author

Chakravarthi Medicharla

## Issues

If you encounter any issues or have feature requests, please file them in the [issues section](https://github.com/Chakravarthy7102/tiptap-highlight/issues).
