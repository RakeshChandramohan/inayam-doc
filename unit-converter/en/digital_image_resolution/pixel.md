## Pixel (px) Measurement Guide & Resolution Converter

### Definition
A **pixel** (symbol: **px**), short for **picture element**, is the fundamental smallest addressable physical point or logical unit in a digital display device or raster image grid.

In CSS and digital web design, **1 CSS pixel** is defined by the W3C as $\frac{1}{96}$ of an inch ($0.2645833 \text{ mm}$). Pixels are used universally to define display resolution ($1920 \times 1080 \text{ Full HD}$, $3840 \times 2160 \text{ 4K UHD}$), camera sensor megapixel ratings, image printing density (**DPI / PPI**), and UI layout sizing.

---

### Quick Pixel Resolution Conversion Reference Table

Search engines frequently feature resolution reference tables in search snippets:

| Display Standard | Resolution (Pixels) | Total Megapixels (MP) | Aspect Ratio | Screen Print Size at 300 DPI |
| :--- | :--- | :--- | :--- | :--- |
| **720p (HD)** | $1280 \times 720$ | 0.92 MP | 16:9 | $4.27 \times 2.40 \text{ in}$ |
| **1080p (Full HD)** | $1920 \times 1080$ | **2.07 MP** | 16:9 | $6.40 \times 3.60 \text{ in}$ |
| **1440p (2K QHD)** | $2560 \times 1440$ | 3.69 MP | 16:9 | $8.53 \times 4.80 \text{ in}$ |
| **4K (UHD)** | $3840 \times 2160$ | **8.29 MP** | 16:9 | $12.80 \times 7.20 \text{ in}$ |
| **8K (FUHD)** | $7680 \times 4320$ | **33.18 MP** | 16:9 | $25.60 \times 14.40 \text{ in}$ |

---

### How to Calculate Pixel Conversions (Formulas & Examples)

To convert between pixels, inches, and millimeters based on Dots Per Inch (**DPI**) or Pixels Per Inch (**PPI**):

- **Pixels to Inches:** $\text{Inches} = \frac{\text{Pixels}}{\text{DPI}}$
- **Inches to Pixels:** $\text{Pixels} = \text{Inches} \times \text{DPI}$
- **Pixels to Millimeters:** $\text{mm} = \left(\frac{\text{Pixels}}{\text{DPI}}\right) \times 25.4$
- **Total Megapixels (MP):** $\text{Megapixels} = \frac{\text{Width (px)} \times \text{Height (px)}}{1,000,000}$

#### Calculation Example:
If a digital photograph image resolution is **$4000 \times 3000$ pixels**, calculate the sensor megapixel rating and the print size at high-resolution **300 DPI**:

1. **Megapixel Calculation:**  
   $$\text{Resolution} = \frac{4000 \times 3000}{1,000,000} = 12.0 \text{ Megapixels (12 MP)}$$

2. **Print Size at 300 DPI:**  
   $$\text{Width} = \frac{4000}{300} = 13.33 \text{ in}, \quad \text{Height} = \frac{3000}{300} = 10.00 \text{ in} \quad (13.33'' \times 10.00'')$$

---

### CSS Pixel vs. Physical Display Pixel (Device Pixel Ratio)
Modern high-density mobile screens (Apple Retina Displays) decouple logical CSS pixels from physical hardware OLED pixels using a **Device Pixel Ratio (DPR)**:

$$\text{Physical Pixels} = \text{CSS Pixels} \times \text{DPR}$$

For example, on an iPhone with a $3\times$ Retina display ($\text{DPR} = 3$), a $100\text{px} \times 100\text{px}$ CSS element renders using $300 \times 300 = 90,000$ physical OLED sub-pixels.

---

### Related Resolution & Digital Unit Converters
Convert digital display metrics across graphic design standards:
- [Byte (B) Converter](https://www.inayam.co/unit-converter/data_storage_si/byte) – Convert image file sizes.
- [Inch (in) Converter](https://www.inayam.co/unit-converter/length/inch) – Convert physical screen dimensions.
- [Centimeter (cm) Converter](https://www.inayam.co/unit-converter/length/centimeter) – Convert print sizes.

---

### Frequently Asked Questions (FAQs)

#### 1. What is the definition of a CSS pixel?
W3C standards define 1 CSS pixel as exactly $\frac{1}{96}$ of an inch ($0.2646 \text{ mm}$).

#### 2. How many pixels are in 1 inch at 300 DPI?
At 300 DPI (Dots Per Inch), 1 linear inch contains **300 pixels** (and 1 square inch contains $90,000 \text{ pixels}$).

#### 3. How many megapixels (MP) is 4K UHD resolution ($3840 \times 2160$)?
4K UHD contains $8,294,400 \text{ pixels}$, which equals **8.29 Megapixels**.

#### 4. How many megapixels is 1080p Full HD resolution ($1920 \times 1080$)?
1080p Full HD contains $2,073,600 \text{ pixels}$, which equals **2.07 Megapixels**.

#### 5. How do I convert pixels to inches?
Divide the pixel dimension by your image DPI: $\text{Inches} = \text{Pixels} / \text{DPI}$.

#### 6. What is the standard web display DPI?
Standard web displays historically use **72 DPI** or **96 DPI**, whereas commercial print requires **300 DPI**.

#### 7. What is Device Pixel Ratio (DPR)?
DPR is the ratio between physical hardware pixels and logical CSS pixels ($\text{Physical} = \text{CSS} \times \text{DPR}$).

#### 8. How do I calculate image file size from pixels?
Multiply width $\times$ height $\times$ color depth (e.g., 24-bit RGB = 3 bytes/pixel) divided by $1,000,000$ for uncompressed Megabytes.
