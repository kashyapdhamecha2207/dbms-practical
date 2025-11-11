// DBMS QUESTION ANSWER (SET - B)

// ANS - 1

CREATE TABLE Hotels (
    hotel_id INT PRIMARY KEY,
    hotel_name VARCHAR(60) UNIQUE,
    city VARCHAR(40),
    rooms_available INT NOT NULL
);


// ANS - 2

// Insert two hotels
INSERT INTO Hotels (hotel_id, hotel_name, city, rooms_available)
VALUES (1, 'Hotel Sunrise', 'Mumbai', 25);

INSERT INTO Hotels (hotel_id, hotel_name, city, rooms_available)
VALUES (2, 'Sea View Inn', 'Goa', 40);

// Update the number of available rooms
UPDATE Hotels
SET rooms_available = 30
WHERE hotel_id = 1;

// Delete a hotel using hotel_id
DELETE FROM Hotels
WHERE hotel_id = 2;

// Calculate total number of rooms available (SUM)
SELECT SUM(rooms_available) AS total_rooms
FROM Hotels;

// Calculate average rooms available (AVG)
SELECT AVG(rooms_available) AS average_rooms
FROM Hotels;
