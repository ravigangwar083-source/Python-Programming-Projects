# Text to Image Converter 🖼️

A simple Python project that converts user-entered text into a PNG image using Pillow. Built in Jupyter Notebook, it demonstrates image creation, text rendering, and word wrapping.

## Features

- Accepts text through user input.
- Creates an 800 × 300 pixel image.
- Displays red text on a white background.
- Wraps text into multiple lines based on available width.
- Uses Pillow's default font.
- Saves the output as a PNG file.

## Technologies Used

- Python
- Jupyter Notebook
- Pillow

## Installation

Install the required library:

```bash
pip install pillow
```

Inside Jupyter Notebook, you can use:

```python
%pip install pillow
```

## How to Run

1. Download or clone this repository.
2. Open `image_convertor.ipynb` in Jupyter Notebook or VS Code.
3. Run the complete text-to-image code cell.
4. Enter your text when prompted.
5. Find `test_sample_24.png` in the notebook's working directory.

## How It Works

1. Takes text input from the user.
2. Creates a blank white image.
3. Loads the default font.
4. Measures text width using `textbbox()`.
5. Wraps words into lines within the available width.
6. Draws each line in red.
7. Saves the image as `test_sample_24.png`.

## Default Settings

| Setting | Value |
|---|---|
| Image size | 800 × 300 pixels |
| Background color | White |
| Text color | Red |
| Font | Pillow default |
| Left and right margins | 50 pixels each |
| Starting vertical position | 50 pixels |
| Line spacing | 25 pixels |
| Output filename | `test_sample_24.png` |

## Example Input

```text
Hello! This image was generated using Python and Pillow.
```

## Console Output

```text
Image generated successfully!
```

## Concepts Practiced

- User input
- Strings and lists
- Loops and conditional statements
- Image creation using Pillow
- Measuring and drawing text
- Word wrapping
- Saving images

## Limitations

- Long text may extend beyond the fixed image height.
- A single word wider than the available width is not split.
- Input line breaks are not preserved.
- Generating another image overwrites the existing output file.

## Author

**Ravi Kumar**  
MCA — Artificial Intelligence & Machine Learning  
Invertis University
