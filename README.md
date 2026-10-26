# Java Image Editor

A simple Java-based image processing project that demonstrates basic image manipulation using Java's built-in image handling libraries.

## Overview

The **Java Image Editor** reads an image from a file, converts it into grayscale, and saves the processed image as a new file. It also includes a utility method to print individual pixel color values to the console.

This project explores image processing fundamentals using Java's `BufferedImage`, `ImageIO`, and `Color` classes.

## Features

- **Grayscale Conversion:** Converts a color image into a grayscale image.
- **Pixel Value Inspection:** Prints the RGB color values of individual pixels to the console.
- **Image File Handling:** Reads and writes images using Java's `ImageIO` API.
- **Preserves Image Dimensions:** The output image retains the original image's width and height.

## Technologies Used

- Java
- `BufferedImage` — for representing and manipulating images.
- `ImageIO` — for reading and writing image files.
- `Color` — for accessing pixel color components.

## Project Structure

```text
ImageEditor/
├── ImageEditor.java
├── image.jpg
└── grayscaleImage.jpg
```

- `ImageEditor.java` — contains the image processing logic.
- `image.jpg` — the input image.
- `grayscaleImage.jpg` — the generated grayscale output.

The input and output images are expected to be accessible from the program's working directory.

## How to Run

### Prerequisites

- Java Development Kit (JDK) installed.
- An input image named `image.jpg`.

### Steps

1. Clone the repository:

   ```bash
   git clone https://github.com/Medha170/Image-Editor/
   ```

2. Navigate to the project directory:

   ```bash
   cd ImageEditor
   ```

3. Place your input image in the project directory and name it `image.jpg`.

4. Compile the Java source file:

   ```bash
   javac ImageEditor.java
   ```

5. Run the program:

   ```bash
   java ImageEditor
   ```

6. Open `grayscaleImage.jpg` to view the output.

## How It Works

1. The program reads the input image using `ImageIO.read()`.
2. The `convertToGrayScale()` method creates a grayscale image with the same dimensions as the original.
3. It iterates through the image's pixels and transfers their RGB values to the grayscale output image.
4. The processed image is saved as `grayscaleImage.jpg` using `ImageIO.write()`.
5. The optional `printPixelValues()` method iterates through the image and prints pixel color components to the console.

## Future Improvements

- Add support for user-provided input and output file paths.
- Implement brightness and contrast adjustments.
- Add image resizing and rotation.
- Build a graphical user interface (GUI).
- Support additional image formats.

## Learning Outcomes

- Understanding image representation in Java.
- Working with pixel-level image data.
- Using Java's built-in image processing and file I/O APIs.
- Practicing loops, methods, exception handling, and object-oriented programming.
