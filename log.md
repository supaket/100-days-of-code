# 100 Days Of Code - Log

### Day 0: May 19, 2019

**Today's Progress**: Setup project and implement initial idea of command line interpreter

**Thoughts:** 

จุดประสงค์ของการเล่น #100DaysOfCode ของผมคืออยากจะ challenge ตัวเองและอยากเรียนรู้ทั้งงานที่ทำอยู่และสิ่งที่ยังไม่เคยเรียนให้กว้างออกไป ปัญหาแรกเลยคือหาโปรเจ็คไม่ได้ แต่ปัญหาต่อมาพอมีไอเดียวผุดขึ้นมาแล้ว ไอเดียโปรเจ็คมันขึ้นมาทีละหลายๆอัน เต็มหัวไปหมด วิธีการ Filter คือจะใช้ value tree ในการคัดกรองมันออกมา หลักๆด้วยเหตุผลของความยืดหยุ่นเช่น microesrvice ที่ใช้ได้หลายภาษา และหลายๆ เทคโนโลยีปนๆกัน อีกทั้งทำแบบ continuous development ได้ได้เรื่อยๆ

ตามกฏคือต้องประกาศให้สาธารณะรู้ว่า ฉันจะเริ่มแล้วนะ โอเคเราเริ่มวันที่ 19 May 2019
และสำหรับหรับ progress เราจะใช้  log.md file และก็ Post ใน twitter และ FB Group ไปพร้อมๆกัน

โปรเจ็คที่จะทำชื่อ generic build flow ยกตัวอย่างง่ายๆ อย่างของ maven หรือ buck build ของ fb แต่ไม่ได้รวมเรื่อง dependencies ด้วย
ที่มาของไอเดียนี้คือในระบบการทำงานด้วย automated ส่วนใหญ่โปรเจ็คจะมี build flow ที่หลายหลาย แต่จะมี life cycle ไม่ต่างกัน ส่วนมากในโปรเจ็คที่ผ่านมาจะ automate กันหรือสร้างเครื่องมีนี้ผ่าน shell script หรืออะไรที่ ฝั่งทาง system admin หรือ infra ทำกันได้ แต่ Dev จะมองไม่ออก ส่วนมากจาก copy พูดแบบไพเราะคือ duplicate code การแก้ปัญหาก็จะเอาลงไปใน Design ด้วยอาจจะเป็น DSL หรือ เอาพวก Markdown มาใช้ในการทำ Grammar ก็อาจจะเป็นไปได้ในทางเลือกหนึ่ง

มาเริ่มกันเลย ด้วยการเลือกภาษาก่อน ในใจมีภาษาในใจคือ Golang กับ Rust ซึ่งเค้าน่าจะเหมาะกับงาน system programming อะไรพวกนี้ แต่งานที่ทำอยุ่ประจำตอนนี้คือภาษา clojure เราจะเอา clojure มาทำตรงนี้ก็คงไม่ผิดอะไรแล้วค่อยไป เพราะตอบโจทย์วัฒถุประสงค์แรกคือ เรียนรู้ที่แล้วทำอยู่แล้ว

วางแผนการทำงาน ผมจะ commit แบบ atomic คือ daily commit ทั้ง 100 วันนี้จะมีแค่ 100 commit ใน 100 วัน เพื่อให้ progress สอดคล้องกับ [log.md](https://github.com/supaket/100-days-of-code/blob/master/log.md) ก็คิดว่า 100 วันข้างหน้าโปรเจ็คจะมี 100 commit.

**Link to work:** [Generic build flow](https://github.com/supaket/gbf/commit/74dcf0c7cf95ce0048e03760e3e7588892f2491e)