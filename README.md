# php-crud-with-css 
PHP CRUD with CSS

## SQL Commands

### Create New Database ✅
    CREATE DATABASE database_name

### Drop Database✅
    DROP DATABASE database_name

### Create table✅
    CREATE TABLE product(
	id int(11) AUTO_INCREMENT PRIMARY KEY,
    product_name varchar(50) NOT NULL
    )
    
### Insert data✅
    INSERT INTO `product`(`id`, `product_name`) VALUES ('1','Hoodie')

### Drop table✅
    DROP TABLE product

### Update Data✅
    UPDATE `product` SET `product_name`='Black Coffe' WHERE `id` = 1

### Delete Data✅
    DELETE FROM `product` WHERE id = 3

### Connection Database✅
    $servername = 'localhost';
    $username = 'root';
    $password = '';
    $database = 'db_hr';

    // Create Connetion
    $conn = new mysqli($servername, $username, $password, $database);

    // Check Connection
    if($conn->connect_error)
    {
        die("Connection Failed". $conn->connect_error);
    }else{
        echo "Tra Error";
    }
   