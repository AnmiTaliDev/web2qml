# web2qml

An AGENTS.md instruction set that turns any AI agent into a smart
Electron/Tauri → QML transpiler. Drop it in your project or paste it
into your agent's context — the AI will analyze your app, map every
component, IPC channel, and CSS variable to idiomatic Qt/QML, and
output a fully structured Qt 6 project.

## What it does

- Detects Electron or Tauri automatically from project files
- Preserves all metadata: name, version, author, window config, icons
- Maps HTML/CSS/JS patterns to native QML components
- Converts IPC channels to C++ signals and Q_INVOKABLE methods
- Translates state management (Redux, Zustand, Pinia, Svelte stores) to QML
- Chooses the right QML stack (Controls 2 / Kirigami / custom)
- Applies QML-specific performance optimizations
- Outputs a complete Qt 6 project with CMakeLists.txt

## Usage

1. Copy `AGENTS.md` into your project root, or paste its contents into
   your agent's system prompt.
2. Give the agent your source files.
3. The agent produces analysis → QML code → README_TRANSPILATION.md.

## Supported input

- Electron (any version)
- Tauri v1 / v2

## Output target

- Qt 6.5 LTS
- QML with QtQuick.Controls 2, Kirigami, or pure custom components

## License

CC BY-SA 4.0
