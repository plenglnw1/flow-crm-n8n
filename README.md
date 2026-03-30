# FlowCRM — n8n workflows

เก็บ workflow JSON สำหรับ **Automation Follow-up**, **Monitoring**, และการเชื่อม **LINE / Laravel** — รัน n8n แยกต่างหากด้วย Docker

---

## Quick Start

1. **โคลน repo**
   ```bash
   git clone <url-ของ-repo-นี้>.git
   cd flow-crm-n8n
   ```
2. **ตั้งค่า environment**
   ```bash
   cp .env.example .env
   ```
   แก้รหัสผ่านใน `.env` ถ้าต้องการ (ค่าเริ่มต้นใช้กับ compose ได้)
3. **ขึ้น stack**
   ```bash
   docker compose up -d
   ```
4. **เปิด UI** — `http://localhost:5678`  
   สร้างบัญชีผู้ใช้ครั้งแรกในเว็บ n8n
5. **นำเข้า workflow** — จากโฟลเดอร์ `workflows/` (เช่น `Action_Stream.json`, `Workflow_Automation_Follow-up.json`)