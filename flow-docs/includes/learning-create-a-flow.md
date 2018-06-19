ยินดีต้อนรับกลับสู่ คำแนะนำสำหรับการเรียนรู้ Microsoft Flow ในบทเรียนนี้ คุณจะเห็นสภาพแวดล้อม Microsoft Flow มากขึ้น และคุณสามารถ**สร้างโฟลว์แรกของคุณ**

เริ่มต้นใช้งาน Microsoft Flow เป็นเรื่องง่าย เนื่องจากมี**เทมเพลตให้เลือก**เป็นจำนวนมาก ซึ่งจะช่วยให้คุณเชื่อมต่อบริการที่คุณใช้อยู่แล้วด้วยวิธีที่สื่อความหมาย  

## <a name="microsoft-flow-templates"></a>เทมเพลต Microsoft Flow
ดูที่[เว็บไซต์ Microsoft Flow](https://ms.flow.microsoft.com) และเปิดเมนู**เทมเพลต** เมื่อคุณเลื่อนผ่านรายการ คุณเห็นว่า Microsoft Flow ให้คุณสามารถเชื่อมต่อกับบริการมากมาย

![เว็บไซต์ Flow -> รายการเทมเพลต](./media/learning-create-a-flow/template-list.png)

## <a name="choose-a-template"></a>เลือกเทมเพลต
**ค้นหาไฟล์แนบ**ทางอีเมลอาจใช้เวลานาน โฟลว์นี้จะช่วยประหยัดเวลาโดย**เก็บไฟล์แนบทั้งหมดของอีเมลคุณ**ลงในโฟลเดอร์ใน OneDrive ของคุณ

เลือกเทมเพลต**บันทึกไฟล์แนบอีเมล Office 365 ลงใน OneDrive for Business**

![อีเมล Office 365](./media/learning-create-a-flow/office-365-email.png)

## <a name="create-and-administer-a-flow"></a>สร้าง และจัดการโฟลว์
นี่คือหนึ่งในเทมเพลต**เพียงคลิกเดียว**ของเรา ที่คุณเพียงแค่ตอบคำถามที่เกี่ยวข้อง**ที่จำเป็นสำหรับการสร้างโฟลว์**เท่านั้น

บนกราฟิกของเทมเพลต มี**คำอธิบาย**ว่าเทมเพลต**ทำอะไร และต้องการอะไร**เพื่อให้บรรลุเป้าหมาย

คุณจะถูกขอให้**ใส่ข้อมูลประจำตัว**สำหรับบริการ **Office 365 Outlook** และ **SharePoint** ถ้าคุณใช้บริการทั้งสองอย่างสม่ำเสมอ คุณจะลงชื่อเข้าใช้บริการทั้งสองอยู่แล้ว

![บันทึกอีเมล Office 365](./media/learning-create-a-flow/save-flow-office-description.png)

1. เลือก**สร้างโฟลว์**
   
    ![คลิกสร้างโฟลว์](./media/learning-create-a-flow/click-create-flow.png)
   
    จากนั้น คุณจะเห็นผลลัพธ์ 
   
    ![สร้างเสร็จเรียบร้อยแล้ว](./media/learning-create-a-flow/create-successful.png)
   
    โฟลว์ได้**สร้างโฟลเดอร์**บน OneDrive ของคุณ ซึ่งจะเก็บ**ทุกไฟล์แนบ**ที่ส่งไปยังอีเมลที่ทำงานของคุณโดยอัตโนมัติ
2. เปิด**โฟลว์ของฉัน**
   
    ![เปิดโฟลว์ของฉัน](./media/learning-create-a-flow/click-my-flows.png)
3. เลือก**โฟลว์ที่คุณเพิ่งสร้าง**เพื่อว่าทำงานอย่างไร
   
    ![เลือกโฟลว์](./media/learning-create-a-flow/click-the-flow.png)
4. คุณจะเห็น**เครื่องหมายถูกสีเขียว** ซึ่งแสดงว่า**โฟลว์ทำงานสำเร็จ** เลือก**สำเร็จ** เพื่อดูประวัติการเรียกใช้และผลลัพธ์
   
    ![โฟลว์ สำเร็จ](./media/learning-create-a-flow/flow-successful.png)
   
    **ทุกส่วนของโฟลว์**สำเร็จ 
   
    ![ประวัติการเรียกใช้](./media/learning-create-a-flow/run-history.png)

## <a name="important-concepts-in-microsoft-flow"></a>แนวคิดที่สำคัญใน Microsoft Flow
บางสิ่งที่ต้องทราบเมื่อสร้างโฟลว์ ทุก ๆ โฟลว์มีสองส่วนที่สำคัญ: **ทริกเกอร์**และ**หนึ่งหรือหลายการดำเนินการ** 

คุณสามารถนึกภาพ**ทริกเกอร์**ว่าเป็นการดำเนินการที่เริ่มต้นโฟลว์ ซึ่งอาจเป็นสิ่งต่าง ๆ เช่น **เมื่อมีอีเมลใหม่**ที่คุณมีตรงนี้ หรือ**เมื่อรายการใหม่ถูกเพิ่ม** ถ้าคุณบังเอิญว่าต้องใช้ SharePoint ทริกเกอร์สามารถกำหนดเป็นตารางเวลาแน่นอน ถ้าคุณใช้ทริกเกอร์ที่เรียกว่า**เกิดขึ้นประจำ** ซึ่งคุณจะได้เรียนรู้ในภายหลัง

**การดำเนินการคือกิจกรรม**ที่คุณต้องการให้เกิดขึ้น เมื่อ**ทริกเกอร์ถูกเรียก** ตัวอย่างเช่น **สร้างไฟล์**จะสร้างไฟล์ใหม่ใน OneDrive

![การดำเนินการเมื่อมีอีเมลใหม่](./media/learning-create-a-flow/trigger-or-action.png)

การดำเนินการอื่น ๆ อาจเป็น การส่ง**อีเมล**, โพสต์**ทวีต**, เริ่มต้น**การอนุมัติ** หรืออื่น ๆ อีกมาก
สิ่งเหล่านี้ทั้งหมดจะเข้ามามีบทบาทต่อไป เมื่อคุณสร้างโฟลว์ของคุณเองตั้งแต่เริ่มต้น 

## <a name="next-lesson"></a>บทเรียนถัดไป
บทเรียนถัดไป จะไปดูที่แอป Microsoft Flow สำหรับอุปกรณ์เคลื่อนที่และความสามารถของแอป 
