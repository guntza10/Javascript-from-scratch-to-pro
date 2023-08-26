# `Javascript-from-scratch-to-pro`

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
