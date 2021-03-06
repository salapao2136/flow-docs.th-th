---
title: เรียนรู้เกี่ยวกับสภาพแวดล้อม Microsoft Flow | Microsoft Docs
description: เรียนรู้วิธีการใช้สภาพแวดล้อมเพื่อแยกโฟลว์ของคุณ
services: ''
suite: flow
documentationcenter: na
author: sunaysv
manager: anneta
editor: ''
tags: ''
ms.service: flow
ms.devlang: na
ms.topic: article
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 11/27/2017
ms.author: sunayv
search.app:
- Flow
search.audienceType:
- flowmaker
- enduser
ms.openlocfilehash: 0e6b410f75f28ba13357878a5cda178bc66b69ff
ms.sourcegitcommit: a20fbed9941f0cd8b69dc579277a30da9c8bb31b
ms.translationtype: HT
ms.contentlocale: th-TH
ms.lasthandoff: 09/12/2018
ms.locfileid: "44690272"
---
# <a name="choosing-an-environment"></a>เลือกสภาพแวดล้อม

บทความนี้จะแนะนำคุณเรื่อง**สภาพแวดล้อม**ของ Microsoft Flow ซึ่งคุณสามารถสร้างและแยกโฟลว์, เกตเวย์, การเชื่อมต่อ และทรัพยากรอื่น ๆ ของคุณได้อย่างปลอดภัย

คุณจะได้เรียนรู้เกี่ยวกับ:

* คุณลักษณะที่สภาพแวดล้อมมอบให้
* การสลับระหว่างสภาพแวดล้อม
* วิธีการสร้างโฟลว์ในสภาพแวดล้อมที่ถูกต้อง

## <a name="environments-overview"></a>ภาพรวมของสภาพแวดล้อม

เมื่อคุณสร้างโฟลว์ คุณเลือกสภาพแวดล้อมสำหรับโฮสต์โฟลว์และทรัพยากรที่โฟลว์ใช้ คุณสามารถแยกสภาพแวดล้อมสำหรับสถานการณ์ที่แตกต่างกัน

## <a name="here-are-a-few-scenarios-for-using-environments"></a>ต่อไปนี้คือตัวอย่างบางสถานการณ์เกี่ยวกับการใช้สภาพแวดล้อม

สถานการณ์สมมติ|คำแนะนำ
-----|-----
คุณต้องการสร้างโฟลว์ที่ใช้การเชื่อมต่อกับ Microsoft Common Data Service|วางโฟลว์ของคุณและ Common Data Service ในสภาพแวดล้อมเดียวกัน ซึ่งช่วยให้มั่นใจว่าข้อมูลทั้งหมดถูกแยกต่างหากภายในสภาพแวดล้อมนั้น (ขอบเขตการแยกจากกัน)
คุณกำลังสร้างโฟลว์สำหรับแผนกทรัพยากรบุคคลของคุณ คุณต้องการให้แน่ใจว่า เฉพาะผู้ใช้ในแผนกทรัพยากรบุคคลของคุณสามารถเข้าถึงโฟลว์ได้|สร้างสภาพแวดล้อม และเพิ่มเฉพาะผู้ใช้ HR ในนั้น วางโฟลว์และทรัพยากรอื่น ๆ ที่โฟลว์ใช้ลงในสภาพแวดล้อมนี้
มีผู้ใช้ในยุโรปที่ใช้โฟลว์เพื่อแสดงข้อมูลของ SharePoint|สร้างสภาพแวดล้อมในยุโรป จากนั้น สร้างโฟลว์ของคุณและการเชื่อมต่อกับ SharePoint ในนั้น สภาพแวดล้อมยุโรปนี้ ช่วยให้ผู้ใช้ที่ยุโรปมีประสิทธิภาพดีที่สุด เนื่องจากทรัพยากรทั้งหมดอยู่ภายในยุโรป (ความใกล้ของข้อมูล)

เพื่อสร้างสภาพแวดล้อม คุณต้องเป็นผู้ดูแล Microsoft Flow ผู้ดูแลระบบควบคุมว่าใครสามารถเข้าถึงสภาพแวดล้อมได้ สำหรับรายละเอียดว่า คุณสามารถสร้างและจัดการสภาพแวดล้อมอย่างไร ดูหัวข้อ[จัดการสภาพแวดล้อม](environments-overview-admin.md)

## <a name="switching-environments"></a>การสลับสภาพแวดล้อม

Microsoft Flow ทำให้ง่ายต่อการสลับระหว่างสภาพแวดล้อม เมื่อคุณสลับสภาพแวดล้อม คุณจะเห็นเฉพาะรายการที่ถูกสร้างขึ้นในสภาพแวดล้อมนั้น ๆ คุณจะไม่เห็น หรือสามารถเข้าถึงรายการในสภาพแวดล้อมอื่น

นี่คือตัวอย่าง

คุณได้สร้างโฟลว์ที่มีชื่อ *NewEmployee* ในสภาพแวดล้อม *Human Resources* ใน [Microsoft Flow](https://flow.microsoft.com) คุณเปิดสภาพแวดล้อม *Sales* โฟลว์ *NewEmployee* จะไม่อยู่ในรายการ เพื่อดูโฟลว์ *NewEmployee* เปิดสภาพแวดล้อม *Human Resources* อย่าลืมว่า กฎเดียวกันใช้กับรายการอื่น ๆ ที่คุณสร้างขึ้นในสภาพแวดล้อมด้วย ซึ่งรวมถึงการเชื่อมต่อ, เกตเวย์, โฟลว์ และอีกมากมาย

ทำตามขั้นตอนเหล่านี้เพื่อสลับสภาพแวดล้อม:

1. ลงชื่อเข้าใช้ [Microsoft Flow](https://flow.microsoft.com)
1. ในมุมบนขวา คุณเห็นรูปภาพที่แสดงโปรไฟล์ของคุณ

   ![รูปโปรไฟล์](./media/environments-overview-maker/default-environment.png)

1. เลือกที่รูปภาพ รายการดรอปดาวน์จะแสดงสภาพแวดล้อมทั้งหมดที่มีสำหรับคุณ สภาพแวดล้อมที่คุณกำลังลงชื่อเข้าใช้อยู่ในขณะนี้ ถูกเครื่องหมายเอาไว้:

   ![รูปรายการของสภาพแวดล้อม](./media/environments-overview-maker/all-environments.png)
1. เพื่อสลับไปยังสภาพแวดล้อมอื่น เลือกสภาพแวดล้อมในรายการ:

   ![เลือกสภาพแวดล้อมเพื่อสลับไป](./media/environments-overview-maker/select-europe.png)
1. Microsoft Flow จะสลับไปยังสภาพแวดล้อมใหม่

## <a name="create-flows-in-the-right-environment"></a>สร้างโฟลว์ในสภาพแวดล้อมที่ถูกต้อง

ก่อนที่คุณสร้างโฟลว์ เลือกสภาพแวดล้อมที่คุณจะเพิ่มโฟลว์และทรัพยากร

> [!NOTE]
> ถ้าคุณสร้างโฟลว์ในสภาพแวดล้อมที่ไม่ถูกต้อง คุณจะจำเป็นต้องลบออก แล้วสร้างใหม่ในสภาพแวดล้อมที่ถูกต้อง

พิจารณาปัจจัยต่อไปนี้เมื่อเลือกสภาพแวดล้อมที่จะโฮสต์โฟลว์ของคุณ:

* คุณสามารถสร้างเกตเวย์ในสภาพแวดล้อมเริ่มต้นเท่านั้น ดังนั้น ถ้าคุณต้องการใช้เกตเวย์เพื่อเชื่อมต่อโฟลว์ของคุณกับข้อมูลภายในองค์กร คุณจำเป็นต้องใช้สภาพแวดล้อมเริ่มต้น
* ฐานข้อมูล Microsoft Common Data Service จะถูกผูกกับสภาพแวดล้อมที่เฉพาะเจาะจง ดังนั้น ถ้าคุณต้องการสร้างโฟลว์ที่ใช้ Common Data Service คุณต้องสร้างโฟลว์ในสภาพแวดล้อมที่โฮสต์ฐานข้อมูล
* คุณจะเห็นสภาพแวดล้อมทั้งหมดที่คุณสามารถแก้ไขทรัพยากร แต่คุณจะต้องขอให้ผู้ดูแลระบบเพิ่มคุณเป็นผู้สร้าง ในทุกสภาพแวดล้อมที่คุณต้องการสร้างโฟลว์

> [!NOTE]
> คุณสามารถสร้างโฟลว์ในสภาพแวดล้อมเริ่มต้นเสมอ

## <a name="next-steps"></a>ขั้นตอนถัดไป

* [สร้างโฟลว์จากเทมเพลต](get-started-logic-template.md)
* [สร้างโฟลว์](get-started-logic-flow.md)
* [ภาพรวมของสภาพแวดล้อมสำหรับผู้ดูแลระบบ](environments-overview-admin.md)
