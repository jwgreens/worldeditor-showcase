# Voxel World Editor
3D World Editor showcase as part of a larger project based on the WrldTmpl8 by Jacco Bikker (see https://jacco.ompf2.com/2021/02/10/voxel-world-template/)


## Overview
worldeditor.cpp implements the core logic for the World Editor in the project. It provides a comprehensive set of features for in-engine voxel/brick-based world editing, including input handling, undo/redo, asset management, and GUI integration.

## Main Features
* NBT Serialization/Deserialization: Implements helper functions for reading and writing world data using the NBT (Named Binary Tag) format, allowing for robust save/load functionality.
* Asset Loading: Loads tiles, big tiles, and sprites from disk, generates preview images, and uploads them as OpenGL textures for use in the editor GUI.
* Input Handling: Processes mouse and keyboard input to support selection, editing, and navigation within the world. Supports multi-selection, add/remove gestures, and hotkeys for undo/redo.
* Editing Operations: Provides functions to add or remove voxels, bricks, tiles, big tiles, and sprites, with logic to avoid redundant operations and track edited regions for undo/redo.
* Undo/Redo System: Maintains a linked list of editor states, allowing users to revert or reapply changes. Manages memory allocation to prevent excessive usage.
* Selection & Gestures: Tracks the currently selected region or object, supports multi-selection and gesture-based editing, and updates rendering parameters for visual feedback.
* GUI Integration: Uses ImGui to render a flexible and interactive editor interface, including asset hotbars, color pickers, camera controls, and statistics.
* World State Management: Handles world resets, state saving/loading, and brick/grid/zeroes buffer management for efficient editing and rendering.

For a video demonstration please checkout my website at https://greenshields.webflow.io