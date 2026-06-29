# plugin-capacities

Plugin รวม Skills สำหรับ **Capacities PKM** ออกแบบมาเพื่อช่วยจัดการ Object Types, Tags, Collections และ Workflow บน Capacities

## Skills

| Skill | วัตถุประสงค์ |
|---|---|
| `skill-mood-tags` | วิเคราะห์อารมณ์จาก Daily Notes และแนะนำ Mood Tag ตาม Yale Mood Meter |

## การติดตั้ง

```bash
# Claude CLI
claude plugin install natthasath/plugin-capacities

# Claude Cowork
/plugin marketplace add natthasath/plugin-capacities
```

## การใช้งาน

### skill-mood-tags

วาง Daily Notes แล้วถามว่า:
- "ควรใช้ mood tag อะไร"
- "tag อารมณ์วันนี้"
- "วิเคราะห์อารมณ์จากบันทึกนี้"

Plugin จะแนะนำ **1 tag** พร้อมโซนและเหตุผลสั้นๆ

### โซนอารมณ์ (Yale Mood Meter)

| โซน | Valence | Arousal | ตัวอย่าง |
|---|---|---|---|
| 🟡 Yellow | บวก | สูง | `#mood-joyful`, `#mood-excited` |
| 🔴 Red | ลบ | สูง | `#mood-stressed`, `#mood-frustrated` |
| 🟢 Green | บวก | ต่ำ | `#mood-calm`, `#mood-reflective` |
| 🔵 Blue | ลบ | ต่ำ | `#mood-sad`, `#mood-unsettled` |