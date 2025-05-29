# Streaming Renderer

## Installation

```bash
npm install streaming-renderer
# or
yarn add streaming-renderer
# or
pnpm add streaming-renderer
```

## Usage

```tsx
import { Xrenderer } from 'streaming-renderer';

function App() {
  return (
    <Xrenderer className="custom-class">
      {`
        # Hello World
        
        This is a markdown content with chart support:
        
        \`\`\`chart
        {
          "type": "line",
          "data": {
            "x": [1, 2, 3, 4, 5],
            "y": [1, 4, 9, 16, 25]
          }
        }
        \`\`\`
      `}
    </Xrenderer>
  );
}
```

## Features

- Markdown rendering with custom styling
- Chart support via @antv/gpt-vis
- Customizable components
- TypeScript support
- React 17+ compatible

## Props

| Prop | Type | Required | Description |
|------|------|----------|-------------|
| children | string | Yes | Xrenderer content to render |
| className | string | No | Custom CSS class name |

## License

MIT
