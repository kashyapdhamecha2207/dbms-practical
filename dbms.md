# 🧠 DBMS QUESTION ANSWER (SET - B)

---

## ✅ **ANS - 1 : Create Table**

```sql
CREATE TABLE Hotels (
    hotel_id INT PRIMARY KEY,
    hotel_name VARCHAR(60) UNIQUE,
    city VARCHAR(40),
    rooms_available INT NOT NULL
);
```

---

## ✅ **ANS - 2 : SQL Operations**

### ➕ **Insert two hotels**

```sql
INSERT INTO Hotels (hotel_id, hotel_name, city, rooms_available)
VALUES (1, 'Hotel Sunrise', 'Mumbai', 25);

INSERT INTO Hotels (hotel_id, hotel_name, city, rooms_available)
VALUES (2, 'Sea View Inn', 'Goa', 40);
```

---

### 🔄 **Update available rooms**

```sql
UPDATE Hotels
SET rooms_available = 30
WHERE hotel_id = 1;
```

---

### ❌ **Delete a hotel by ID**

```sql
DELETE FROM Hotels
WHERE hotel_id = 2;
```

---

### 🧮 **Calculate total rooms (SUM)**

```sql
SELECT SUM(rooms_available) AS total_rooms
FROM Hotels;
```

---

### 📊 **Calculate average rooms (AVG)**

```sql
SELECT AVG(rooms_available) AS average_rooms
FROM Hotels;
```

---

**💡 Summary:**  
This set demonstrates **table creation**, **data insertion**, **update**, **deletion**, and **aggregate functions (SUM, AVG)** in SQL — all core DBMS operations.
