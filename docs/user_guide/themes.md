# Color Themes

The Chess Board Drawer application offers several elegant color themes for your chess board. Each theme provides a unique visual style while maintaining excellent contrast between squares.

## Available Themes

The following themes are available in the application:

### Classic
<div style="display: flex; align-items: center; margin-bottom: 20px;">
    <div style="width: 100px; height: 100px; display: grid; grid-template-columns: 1fr 1fr; grid-template-rows: 1fr 1fr; margin-right: 20px;">
        <div style="background-color: #EEEED2;"></div>
        <div style="background-color: #769656;"></div>
        <div style="background-color: #769656;"></div>
        <div style="background-color: #EEEED2;"></div>
    </div>
    <div>
        <p>The traditional chess board colors used in many tournaments.</p>
        <ul>
            <li>Light squares: <code>#EEEED2</code> (cream)</li>
            <li>Dark squares: <code>#769656</code> (forest green)</li>
        </ul>
    </div>
</div>

### Vintage
<div style="display: flex; align-items: center; margin-bottom: 20px;">
    <div style="width: 100px; height: 100px; display: grid; grid-template-columns: 1fr 1fr; grid-template-rows: 1fr 1fr; margin-right: 20px;">
        <div style="background-color: #E8D0AA;"></div>
        <div style="background-color: #B67C4A;"></div>
        <div style="background-color: #B67C4A;"></div>
        <div style="background-color: #E8D0AA;"></div>
    </div>
    <div>
        <p>A warm, wooden appearance reminiscent of antique chess sets.</p>
        <ul>
            <li>Light squares: <code>#E8D0AA</code> (light tan)</li>
            <li>Dark squares: <code>#B67C4A</code> (medium brown)</li>
        </ul>
    </div>
</div>

### Purple
<div style="display: flex; align-items: center; margin-bottom: 20px;">
    <div style="width: 100px; height: 100px; display: grid; grid-template-columns: 1fr 1fr; grid-template-rows: 1fr 1fr; margin-right: 20px;">
        <div style="background-color: #E6D5F5;"></div>
        <div style="background-color: #9966CC;"></div>
        <div style="background-color: #9966CC;"></div>
        <div style="background-color: #E6D5F5;"></div>
    </div>
    <div>
        <p>A modern, vibrant purple theme with excellent contrast.</p>
        <ul>
            <li>Light squares: <code>#E6D5F5</code> (light lavender)</li>
            <li>Dark squares: <code>#9966CC</code> (amethyst purple)</li>
        </ul>
    </div>
</div>

### Gray
<div style="display: flex; align-items: center; margin-bottom: 20px;">
    <div style="width: 100px; height: 100px; display: grid; grid-template-columns: 1fr 1fr; grid-template-rows: 1fr 1fr; margin-right: 20px;">
        <div style="background-color: #E8E8E8;"></div>
        <div style="background-color: #707070;"></div>
        <div style="background-color: #707070;"></div>
        <div style="background-color: #E8E8E8;"></div>
    </div>
    <div>
        <p>A minimalist grayscale theme for a clean, professional look.</p>
        <ul>
            <li>Light squares: <code>#E8E8E8</code> (light gray)</li>
            <li>Dark squares: <code>#707070</code> (medium gray)</li>
        </ul>
    </div>
</div>

### Blue
<div style="display: flex; align-items: center; margin-bottom: 20px;">
    <div style="width: 100px; height: 100px; display: grid; grid-template-columns: 1fr 1fr; grid-template-rows: 1fr 1fr; margin-right: 20px;">
        <div style="background-color: #D6E5FA;"></div>
        <div style="background-color: #5D8BF4;"></div>
        <div style="background-color: #5D8BF4;"></div>
        <div style="background-color: #D6E5FA;"></div>
    </div>
    <div>
        <p>A calming blue theme that's easy on the eyes.</p>
        <ul>
            <li>Light squares: <code>#D6E5FA</code> (pale blue)</li>
            <li>Dark squares: <code>#5D8BF4</code> (royal blue)</li>
        </ul>
    </div>
</div>

### Red
<div style="display: flex; align-items: center; margin-bottom: 20px;">
    <div style="width: 100px; height: 100px; display: grid; grid-template-columns: 1fr 1fr; grid-template-rows: 1fr 1fr; margin-right: 20px;">
        <div style="background-color: #F5D5D5;"></div>
        <div style="background-color: #D35D6E;"></div>
        <div style="background-color: #D35D6E;"></div>
        <div style="background-color: #F5D5D5;"></div>
    </div>
    <div>
        <p>A vibrant red theme for a bold, striking appearance.</p>
        <ul>
            <li>Light squares: <code>#F5D5D5</code> (light pink)</li>
            <li>Dark squares: <code>#D35D6E</code> (raspberry red)</li>
        </ul>
    </div>
</div>

## Selecting a Theme

To change the theme of your chess board:

1. Locate the **Themes** section in the UI (at the bottom of the application)
2. Click on any of the theme buttons to apply it
3. The board will update immediately with the new colors

## Adding Custom Themes

If you're a developer, you can easily add your own custom themes to the application by modifying the `color_themes` dictionary in the source code:

```python
# Add your custom theme
color_themes["MyTheme"] = {"light": "#YOURCOLOR1", "dark": "#YOURCOLOR2"}
```

When choosing colors for a custom theme, consider these guidelines:

- Ensure high contrast between light and dark squares
- Test your theme for visibility of chess pieces (especially in the chess game component)
- Use web-safe colors or hexadecimal color codes

## Theme Implementation Details

Each theme in the application is implemented as a dictionary entry with two color values:

```python
color_themes = {
    "Classic": {"light": "#EEEED2", "dark": "#769656"},
    # Other themes...
}
```

When a theme is selected, the application:

1. Retrieves the light and dark colors from the theme dictionary
2. Redraws the entire board using the new colors
3. Updates the UI to highlight the currently selected theme

For more details on the implementation, see the [`change_theme()`](../reference/chess_board_drawer.md#change_theme) function in the API reference.