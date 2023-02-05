คู่มือและวิธีการ
- เตรียม jupyter notebook โดย download anaconda มาเพื่อใช้ jupyter notebook
- ลง python version 3.9
- ทำการลง library ต่างๆให้เรียบร้อย
- ใช้คำสั่ง pip3 install scikt-learn numpy os random math datetime collection pandas PTL pathlib joblib
- ใช้คำสั่ง pip3 install torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/cu113

วีธีการ
- สามารถรันแต่ละเซลล์ตามขึ้นตอนไล่ลงจากขึ้นลงมาจนสิ้นสุดได้เลยจะประกอบไปด้วยการ นำ dataset มาใช้งาน การทำ data preprocessing การทำ pre-train และ train ตัว model ทั้ง 5 model รวมถึงการประเมินผลรวมถึงการทดลองทำนายกับ unseen data จริงๆ
- โดยต้องทำการใส่ path ที่ตามกับ dataset ทั้งสองคือ images_path และ anno_path ตามไฟล์ที่แนบไปให้
- การทำการทดลองในหลายๆ method ในการปรับรูปต้องทำการปรับ ในส่วนของการ preprocessing เช่น จะทำการทดลองกับ sharpenBrightnessContrast ต้องทำการเรียกใช้ฟังก์ชั่น sharpenBrightnessContrast ในหัวข้อที่เป็น Experiment image enhancement
- การทดลองกับ unseen data จะอยู่ในหัวข้อ Test with unseen data ซึ่งจะได้คำตอบที่อยู่ในหัวข้อ Predicted class ซึ่งจะให้ output เป็น value ของค่าความน่าจะเป็นของ class ที่มากที่สุด
- สามารถทำการโหลด model ได้โดยไม่ต้องทำการ train ใหม่เพราะใช้เวลาค่อนข้างนานทำการโหลด model ได้ในหัวข้อ Load model to use
