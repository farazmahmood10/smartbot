<?php
header("Content-Type: application/json");
$_POST = json_decode(file_get_contents('php://input'), true);

$response = [
    "speech" => "Dev server has received the request",
    "displayText" => "Dev server has received the request",
    "data" => $_POST,
    "source" => "dev_server"
];

echo json_encode($response); ?>
