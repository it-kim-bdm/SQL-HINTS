# SQL-HINTS
JUST REMINDER, IF I FORGOT


### BUAT TABLE DENGAN STRUKTUR KOLOM YANG SAMA
```sql
CREATE TABLE cuti_new_request LIKE cuti_new;
```


### MOVE FROM CUTI REQUEST TO CUTI REAL
```sql
INSERT INTO cuti_new SELECT * FROM cuti_new_request WHERE id_cuti='$id_cuti';
```

### DELETE DATA ON CUTI REQUEST IF ALL ACC DONE
```sql
DELETE FROM cuti_new_request WHERE id_cuti='$id_cuti';
```
