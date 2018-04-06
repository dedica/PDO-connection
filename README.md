# PDO-connection

try {
    $pdo = new PDO("mysql:host=localhost;dbname=toys", "root", "root");
} catch (PDOException $e) {
    echo "Failed to get DB handle: " . $e->getMessage() . "\n";
    exit;
}

$query = $pdo->prepare("SELECT * FROM toy_products");
$query->execute();
$data = $query->fetchAll();

echo "<pre>";
print_r($data);
echo "</pre>";
