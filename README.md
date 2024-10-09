# ComputerVisionTask
Semester 2 Computer vision Quiz 1 Task

# **Task1 Explanation**

The differences between the original image, the shrunk image, and the zoomed image can be explained by considering the processes involved in shrinking and zooming and how they affect image quality:

# **1. Loss of Detail When Shrinking**
Shrinking an image from 1250 DPI to 100 DPI means reducing the number of pixels, which throws away a lot of the original details.
With fewer pixels, the smaller image can’t capture fine details, sharp edges, or tiny textures as well as the original. This makes the image look more blurred and less defined.
# **2. Blurry Look When Enlarging Again**
When you zoom the 100 DPI image back to 1250 DPI, the software has to "guess" what the extra pixels should look like using a method called bilinear interpolation. This involves averaging nearby pixels to fill in the gaps.
However, since a lot of details were lost during shrinking, the guessed pixels can't bring back the original sharpness and detail, making the enlarged image look softer or blurrier.
# **3. Blurring Due to Interpolation**
Bilinear interpolation is a fast way to enlarge images, but it often causes blurring because it smooths out the details by averaging the colors of nearby pixels.
The original high-resolution image had much crisper details that are difficult to recreate once they’ve been lost.
# **4. Jagged Edges (Aliasing)**
When you reduce the size of an image, it can lead to aliasing, which creates jagged edges or strange patterns, especially in areas with fine textures or lines.
These jagged edges stay in the image even when you zoom back up, making the enlarged image look different from the original.
# **5. Pixelation**
When zooming the shrunken image back up, the original pixel density and details are gone. The new pixels are created based on estimations, not the original information.

# **Conclusion:**
When  shrink an image, Image lose important details. Enlarging it again can’t bring back those lost details because the process relies on estimations, which tend to blur sharp features and make the image look less defined. This results in visible differences like blurring, loss of fine details, jagged edges, and pixelation in the zoomed image.





# **Explanation Task 2**
The main differences between log transformation and power-law (gamma) transformation come from how they change the brightness and contrast in an image. Here’s why they work differently:

### 1. **Log Transformation**
   - **How It Works:** The formula is \( s = c \cdot \log(1 + r) \), where \( c \) is a constant, and \( r \) is the original pixel brightness.
   - **What It Does:** Log transformation brightens the darker parts of the image while toning down the brighter areas. It’s great for showing details in shadows or dark regions.
   - **When It’s Useful:** It works well for images with a lot of dark areas where details are hard to see. It helps bring out those details without making the bright areas too bright.

### 2. **Power-Law (Gamma) Transformation**
   - **How It Works:** The formula is \( s = c \cdot r^\gamma \), where \( c \) is a constant, and \( \gamma \) (gamma) controls how the brightness changes.
   - **What It Does:** You can adjust \( \gamma \) to change how the brightness and contrast look. If \( \gamma < 1 \), it makes dark areas brighter; if \( \gamma > 1 \), it makes bright areas even brighter.
   - **When It’s Useful:** It’s more flexible than log transformation. You can use it to either brighten dark areas or emphasize bright areas, depending on the value of \( \gamma \). This makes it suitable for a wide range of images.

### Why They Look Different:
1. **How They Change Brightness:**
   - **Log Transformation:** Focuses on brightening darker parts, which makes it better at revealing details in shadows. It reduces the intensity of bright areas because it compresses the range of brighter values.
   - **Power-Law Transformation:** Gives more control over which part of the image you want to change. By adjusting \( \gamma \), you can choose to make either dark or bright areas stand out more.

2. **Adjusting Contrast:**
   - **Log Transformation:** Has a fixed way of changing brightness, so you can’t fine-tune it as much.
   - **Power-Law Transformation:** Lets you control the contrast by adjusting \( \gamma \), making it more versatile for enhancing different parts of the image.

3. **Best Uses:**
   - **Log Transformation:** Good for images with lots of dark details that need to be highlighted.
   - **Power-Law Transformation:** Works well for various types of images because you can adjust \( \gamma \) to get the desired effect.

### Conclusion:
- **Log transformation** is great for making dark areas clearer but can make bright areas less intense.
- **Power-law transformation** gives more control over the image’s appearance by adjusting \( \gamma \), allowing you to enhance either dark or bright areas.

The key difference is in how each method changes the brightness, which affects their ability to reveal details and adjust contrast in different parts of the image.





# *Task4 Histogram**
"Note: In GitHub, the image is not displaying correctly. I have uploaded a screenshot of the result named Task4_Histogram Image.png."
![Task 4 Histogram Equalization Result](Task4_Histogram%20Image.png)

