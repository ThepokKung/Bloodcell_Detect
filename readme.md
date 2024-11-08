# Blood Cell Detection
ทำการนับ Cell โดยใช้ image processing จากรูป

![BloclCell](/image_for_readme/bloodcell.bmp)

**โดยจะใช้ Python openCV ในการแก้ปัญหา**

# Table of content
- [Blood Cell Detection](#blood-cell-detection)
- [Table of content](#table-of-content)
- [ขั้นตอนการแก้ปัญหา](#ขั้นตอนการแก้ปัญหา)
- [Contract](#contract)

# ขั้นตอนการแก้ปัญหา
 * 1. ทำการอแปลรูปเดิม ให้อยู่ในรูปแบบ grayscale เพื่อให้ง่ายต่อการจำแนกตัว cell
 * 2. แปลงรูปภาพจาก .bmp ให้่เป็นรูป .png เพื่อให้เราสามารถใช้ HSV format ได้ โดยเราจะได้รูป bloodcell_gray.png มาดังรูป
  
![bloodcell_gray.png](/image_for_readme/bloodcell_gray.png)
  
  * 3. ทำการแปลงให้อยู่ในรูป HSV เพื่อที่จะเราจะได้ตรวจสอบ cell จากจุดกลาง โดยจะได้ดังรูป 
  
![HSV](/image_for_readme/HSV.png)

  * 4. จะสังเกตุได่ว่าภาพจาก HSV ของเรานั้นจุดตรงการจะมีสี **ดำ** โดยเราได้ทำการ mask จุดโดยใช้ Value (brightness level) ที่ 30 - 75 โดยจะได้รูปดังรูปนี้

![orivmask](/image_for_readme/orivmask.png)

  * 5. ทำการนับ Cell แต่ละ cell ที่ขึ้นตามรูป
  
![final](/image_for_readme/final.png)

# Contract 

Kraiwich Vichakhot - [@ThepokKung](https://www.github.com/ThepokKung)
