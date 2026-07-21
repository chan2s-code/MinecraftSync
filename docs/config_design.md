# Config Design

## 목적

프로그램의 모든 설정을 config.json에서 관리한다.

---

## config.json

{
    "minecraft": {

    },

    "google_drive": {

    },

    "backup": {

    },

    "program": {

    }

}

---

## minecraft

| 설정 | 설명 |
|------|------|
| world_path | 월드 저장 위치 |

---

## google_drive

| 설정 | 설명 |
|------|------|
| folder_id | Google Drive 폴더 ID |

---

## backup

| 설정 | 설명 |
|------|------|
| temp_path | 임시 ZIP 저장 위치 |
| keep_backup_count | Google Drive에 유지할 백업 개수 |

---

## program

| 설정 | 설명 |
|------|------|
| log_level | 로그 출력 수준 |