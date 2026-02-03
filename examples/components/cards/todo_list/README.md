# Todo List Component

This is an example todo list component created with LVGL XML.

## Features

- Interactive checkboxes for marking tasks as complete
- Visual feedback when tasks are checked (disabled/strikethrough styling)
- Dark theme support
- Progress counter showing completed tasks
- Clean, card-based design consistent with other LVGL components

## Component Structure

### Files
- `todo_list.xml` - Main todo list card component
- `todo_item.xml` - Individual todo item component (optional, for reference)

### Global Subjects

The following subjects are defined in `examples/globals.xml`:

```xml
<int name="todo_task1_done" value="0" help="0:not done, 1:done" />
<int name="todo_task2_done" value="1" help="0:not done, 1:done" />
<int name="todo_task3_done" value="0" help="0:not done, 1:done" />
<int name="todo_task4_done" value="0" help="0:not done, 1:done" />
<int name="todo_task5_done" value="0" help="0:not done, 1:done" />
<int name="todo_completed_count" value="1" help="Number of completed tasks" />
```

## Usage

### In a Screen

```xml
<screen>
  <view flex_flow="column">
    <todo_list />
  </view>
</screen>
```

### Viewing the Example

1. Open the LVGL Editor or Online Viewer (https://viewer.lvgl.io/)
2. Load the `examples/screens/todo_list.xml` screen to see the todo list standalone
3. Or load the `examples/screens/elements.xml` screen to see it with other components

## Customization

You can customize the todo list by:

1. **Modifying tasks**: Edit the task text in `todo_list.xml`
2. **Adding/removing tasks**: Add or remove task rows and update the progress counter
3. **Changing colors**: Modify the `panel_light` and `panel_dark` styles
4. **Styling**: Adjust fonts, padding, and other style properties

## Example Tasks

The example includes 5 common development tasks:
1. Review pull requests
2. Update documentation
3. Fix reported bugs
4. Prepare release notes
5. Test on target device
