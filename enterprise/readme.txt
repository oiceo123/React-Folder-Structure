โปรเจกต์ขนาดใหญ๋

node_modules            เก็บ package ต่างๆ
public                  เก็บไฟล์ต่างๆ ที่สามารถเผยแพร่ได้ เช่น index.html, logo แต่ไม่ควรใช้ folder นี้ในการเก็บไฟล์รูปภาพต่างๆ
.gitignore              เป็นไฟล์ที่ไว้บอกให้ git รู้ว่าจะไม่ให้ git track ไฟล์ไหนบ้าง
package.json            เป็นไฟล์ไว้เก็บรายละเอียดของโปรเจกต์ และ เก็บ dependency ต่างๆที่โปรเจกต์ใช้งาน
README.md               เป็นไฟล์ที่เอาไว้เขียนรายละเอียดต่างๆ ที่เราต้องการเก็บไว้อ่าน (สามารถใช้งานร่วมกับ git ได้)
src                     เป็น folder หลักที่ใช้ในการเขียนโปรแกรม เก็บไฟล์ที่เกี่ยวข้องกับการทำงานของเว็บไว้ทั้งหมด 

src/asset               เก็บรูปภาพทั้งหมดในโปรเจกต์ ซึ่งควรแยกย่อยเป็น folder อีกทีนึง
src/assets/brand        เก็บรูปภาพที่เกี่ยวข้องกับ brand เท่านั้น (ไม่แน่ใจ)
src/assets/images       เก็บรูปภาพของแต่ละหน้า ทำให้ง่ายต่อการนำไปใช้งานในโปรเจกต์
src/assets/svg          เก็บรูปภาพของแต่ละหน้า ซึ่งจะเก็บในนามสกุล svg เท่านั้น
src/asset/global.css    ไฟล์ css ที่ใช้ทำ style ในเว็บของเรา

src/components          เก็บ components ทั้งหมดในโปรเจกต์ ซึ่งควรแยกย่อยเป็น folder อีกทีนึง
src/components/Buttons  เก็บ components, css ที่เกี่ยวข้องกับ Buttons เท่านั้น เพื่อให้ง่ายต่อการใช้งานในโปรเจกต์
src/components/Input    เก็บ components, css ที่เกี่ยวข้องกับ Input เท่านั้น เพื่อให้ง่ายต่อการใช้งานในโปรเจกต์
src/components/layouts  เก็บ components, css ที่เกี่ยวข้องกับ layouts เท่านั้น เพื่อให้ง่ายต่อการใช้งานในโปรเจกต์
                        ซึ่งใน layouts จะเก็บพวก Navbar, Sidebar, Header, Footer ซึ่งมักจะถูกใช้ซ้ำๆ ในหลายหน้า

src/context             เก็บ Context ของแต่ละหน้า
src/context/tests       เก็บไฟล์สำหรับใช้ Test Context

src/data                เก็บไฟล์ที่รวมรวมข้อมูลทั้งหมดไว้ในรูปของ Block Data ซึ่งเอาไว้ใช้ในเว็บของเรา

src/hooks               ใช้สำหรับเก็บ hook ต่างๆที่สร้างขึ้นมาเอง
src/hooks/tests         เก็บไฟล์สำหรับใช้ Test hook ต่างๆ

src/lib                 เก็บไฟล์ที่เกี่ยวข้องกับ lib 3 party ที่เอามาใช้ในโปรเจกต์ เพื่อที่เวลาเราจะ update จะได้แก้แค่ไฟล์เดียวไม่ต้องไปไล่แก้ทีละไฟล์

src/utils               เก็บ function ทั่วไป และ utility ต่างๆ ซึ่งจะถูกใช้ซ้ำในส่วนต่างๆ ของเว็บ
src/utils/tests         เก็บไฟล์สำหรับใช้ Test utility ต่างๆ

src/pages               เก็บ page ของแต่ละหน้าไว้
src/pages/About.jsx     หน้าเว็บของ About
src/pages/Home.jsx      หน้าเว็บของ Home
src/pages/Login.jsx     หน้าเว็บของ Login
src/pages/...           หน้าเว็บของ  ... (อะไรก็ได้ที่สามารถทำเป็น page ได้)

*** ซึ่งที่เราไม่ต้องเก็บเป็น folder เพราะว่าเราได้แยกสิ่งต่างๆ ที่เกี่ยวข้องกับแต่ละหน้าไปไว้ที่ features แล้ว ***

src/features                        เก็บ folder ต่างๆที่อ้างอิงจากไฟล์ใน folder pages
src/features/product                เก็บ folder ต่างๆที่ page product ต้องนำไปใช้ เช่น logics, components, assets เป็นต้น
src/features/product/assets         เก็บรูปภาพที่ page product ต้องนำไปใช้
src/features/product/components     เก็บ component ที่ page product ต้องนำไปใช้
src/features/product/context        เก็บ context ที่ page product ต้องนำไปใช้
src/features/product/services       เก็บ service ที่ page product ต้องนำไปใช้
src/features/product/index.jsx      ทำหน้าที่สร้างหน้า page product ไว้ก่อน แล้วค่อยให้ไฟล์ที่ชื่อ Product.jsx ใน folder pages import ไปใช้งาน
                                    ทำแบบนี้เพื่อที่จะทำให้ในส่วนของ folder pages ไม่ลก
