# DATA STRUCTURES - PROCESSING IMAGES

This repository contains the Processing Images project, which is the final project of the Data Structures Course from Cornell University's Python Programming certificate program.

## Overview

This project demonstrates Python Data Structure concepts through image manipulation, focusing on:
- Objects (RGB pixel objects)
- Lists, Tuples
- Nested Lists (2D image buffers)
- Dictionaries

## Features

The application provides various image processing functions that work with images represented as 2D tables of RGB objects:

### Core Functions
- **mono** - Convert images to greyscale or sepia tone
- **dered** - Remove all red values from the image
- **flip** - Reflect images horizontally or vertically
- **transpose** - Swap rows and columns
- **rotate** - Rotate images 90 degrees left or right

### Advanced Functions (Optional)
- **vignette** - Apply corner darkening effect
- **blur** - Blur images with configurable radius
- **pixellate** - Create blocky pixelated effect

## Project Structure

```
processing-images/
├── pictool.py          # Main application with CLI support
├── plugins.py          # Image processing functions
├── images/             # Sample input images
└── solutions/          # Expected output examples
```

## Usage

### Command Line Syntax

```bash
python pictool.py <command> [options] <input> [output]
```

### Examples

```bash
# Convert to greyscale
python pictool.py mono images/Walker.png output.png

# Convert to sepia tone
python pictool.py mono --sepia=True images/Walker.png output.png

# Flip horizontally
python pictool.py flip images/Walker.png output.png

# Flip vertically
python pictool.py flip --vertical=True images/Walker.png output.png

# Rotate right
python pictool.py rotate --right=True images/Walker.png output.png

# Remove red channel
python pictool.py dered images/Walker.png output.png

# Transpose image
python pictool.py transpose images/Walker.png output.png
```

## Sample Images

The project includes several test images:
- blocks.png
- debug.png
- Goldhill.png
- home.png
- Japan.png
- rocket.png
- Walker.png

## Dependencies

- Python 3.x
- PIL (Pillow)
- introcs module

## Author

Sravan Kumar Nuthalapati  
Date: 01/31/2026
