DROP DATABASE task_2;
create database task_3;

use task_3;

CREATE TABLE products (
    id INT AUTO_INCREMENT PRIMARY KEY,
    product_name VARCHAR(100) NOT NULL,
    price DECIMAL(10, 2)
);

describe products;

ALTER TABLE products
ADD CONSTRAINT chk_price_positive CHECK (price > 0);

INSERT INTO products (product_name, price) VALUES
('Laptop', 999.99),
('Smartphone', 599.99),
('Tablet', 299.99),
('Keyboard', 19.99),
('Mouse', 14.99),
('Desk Lamp', 24.99),
('Speakers', 9.99);

ALTER TABLE products
MODIFY COLUMN product_name VARCHAR(120) NOT NULL;

select*from products;
