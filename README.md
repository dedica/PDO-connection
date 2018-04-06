# PDO-connection

## try {
&nbsp;&nbsp;&nbsp;&nbsp;## $pdo = new PDO("mysql:host=localhost;dbname=toys", "root", "root");
## } catch (PDOException $e) {
&nbsp;&nbsp;&nbsp;&nbsp;## echo "Failed to get DB handle: " . $e->getMessage() . "\n";
&nbsp;&nbsp;&nbsp;&nbsp;## exit;
## }

## $query = $pdo->prepare("SELECT * FROM toy_products");
## $query->execute();
## $data = $query->fetchAll();

## echo "<pre>";
## print_r($data);
## echo "</pre>";
