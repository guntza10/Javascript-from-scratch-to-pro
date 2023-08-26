# `Javascript-from-scratch-to-pro`

# `An Introduction to JavaScript`

## `What is JavaScript?`

- ตอนแรกถูกสร้างขึ้นสำหรับทำ website
- เป็น script ที่สามารถเขียนบน html และทำงาน auto เมื่อโหลดหน้า website
- execute เป็น plain text โดยไม่ต้องจำเป็นต้องเตรียมหรือcompileอะไรเลยในการที่จะ run
- `ECMAScript` เป็นข้อกำหนด standart ของ js
- run ได้ทุก platform ทั้ง browser,server และ device ต่างๆ ที่มี `JavaScript engine`
- บน browser จะมี embedded engine ที่เรียกว่า `JavaScript virtual machine` (เอาไว้ใช้ run js)
- แต่ละ engine ก็จะมี codename ที่ใช้แตกต่างกัน
  - `V8` – in Chrome, Opera and Edge.
  - `SpiderMonkey` – in Firefox.
  - `Chakra` – in IE.
  - `JavaScriptCore`, `Nitro` and `SquirrelFish` for Safari

### `How do engines work?`

- engine อ่าน script
- convert script ไปเป็น machine code
- machine code run (fast)

## `What can in-browser JavaScript do?`

- ใน browser js สามารถทำทุกย่างที่เกี่ยวกับ webpage manipulation,interaction user,webserver
- add new html,change the existing content, modify styles
- การ react ต่างๆกับ user เช่น run on mouse clicks, pointer movements, key presses.
- send request ข้าม network เพื่อ remote server,download and upload files
- get,set cookies
- ask questions to the visitor, show messages.
- เก็บ data ไว้ที่ client-side (`local storage`)

## `What CAN’T in-browser JavaScript do?`

- js ไม่สามารถ direct access OS functions ได้
  - ไม่สามารถ read,write files บน hard disk ได้
  - modern browser allow การทำงานกับ file แต่จะ limit access
  - และจะให้ access ถ้า user ทำ action บางอย่างเท่านั้น
  - เช่น การ browse file ผ่าน `<input>`
- การใช้ camera,microphone และ other devices ต้อง require permission
  - เพราะฉะนั้นการเปิด web ขึ้นมา อาจจะไม่สามารถแอบเปิด camera,microphone และ other devices ได้ ถ้า user ไม่ allow permission
- js จาก คนละ tab,window กัน ไม่สามารถ access หากันได้ (ถ้าเป็นคนละ web กัน) ซึ่งสิ่งนี้เรียกว่า `Same Origin Policy`
  - ยกตัวอย่าง tab,window ของเว็บ `http://anysite.com` ไม่สามารถ access tab,window ของเว็บ `http://gmail.com` ได้
  - ซึ่ง `Same Origin Policy` ก็จะป้องกันการขโมยข้อมูลจากคนละ tab,window ได้
- js สามารถ communicate ผ่าน net ไปยัง server ของหน้าที่เปิดอยู่ตอนนี้ได้อย่างง่ายดาย
  - แต่ ability ในการรับ data จาก website หรือ domain อื่นๆ จะลดลง
  - แต่การจะทำแบบนั้นได้ ต้อง require explicit agreement (ที่ต้องแนบมากับ HTTP headers) จากระยะไกล
  - นี่เป็น safety limitation (ข้อจำกัดด้านความปลอดภัย)
  - safety limitation นี้จะใช้ไม่ได้ ถ้าใช้ js นอก browser
  - เช่น บน server modern browser ยัง allow plugin/extension ที่อาจจะขอ permissions เพ่ิมเติม

## `What makes JavaScript unique?`

- ทำงานร่วมกับ HTML/CSS
- ทำงานได้กับทุก browser
- นอกจากทำ website แล้วยังสามารถใช้ทำ servers, mobile applications ได้อีกด้วย

# `JavaScript Fundamentals`
