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
This can lead to a pixelated look where areas that used to have fine details now appear blocky or overly smooth.

# **Conclusion:**
When  shrink an image, Image lose important details. Enlarging it again can’t bring back those lost details because the process relies on estimations, which tend to blur sharp features and make the image look less defined. This results in visible differences like blurring, loss of fine details, jagged edges, and pixelation in the zoomed image.
