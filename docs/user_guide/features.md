# Features

The Chess Board Drawer includes several features that make it flexible and user-friendly.

## Color Themes

The application comes with six built-in color themes:

| Theme | Light Squares | Dark Squares | Description |
|-------|--------------|--------------|-------------|
| Classic | `#EEEED2` | `#769656` | Traditional chess board colors |
| Vintage | `#E8D0AA` | `#B67C4A` | Antique wood-like appearance |
| Purple | `#E6D5F5` | `#9966CC` | Modern purple-themed board |
| Gray | `#E8E8E8` | `#707070` | Minimalist grayscale design |
| Blue | `#D6E5FA` | `#5D8BF4` | Calming blue palette |
| Red | `#F5D5D5` | `#D35D6E` | Vibrant red color scheme |

To change the theme, simply click on any theme button in the UI.

## Board Size

The board size can be adjusted from 4×4 to 16×16:

- Click the `-` button to decrease the size
- Click the `+` button to increase the size

The application automatically adjusts the square sizes to fit the screen.

## Animation Control

The animation toggle controls how the board is drawn:

- **OFF**: The board appears instantly (default)
- **ON**: You can see the drawing process animated

## Chess Game Integration

Clicking the "Play Game" button launches the associated chess game with your selected theme. This integrates with the `chess_game` module, which must be in the same directory.

## Board Labels

For standard 8×8 boards, the application automatically adds:

- Column labels (a-h)
- Row numbers (1-8)

This makes the board suitable for standard chess notation.

## Error Handling

The application includes robust error handling:

- Graceful exit with Ctrl+C
- Exception reporting
- Protection against invalid board sizes