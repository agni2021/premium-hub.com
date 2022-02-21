<?php
$name = $_REQUEST['Name'];
$email = $_REQUEST['Email'];
$message = $_REQUEST['msg'];


if (empty($name) || empty($email) || empty($message)){
  echo('please fill all the fields');
} 
else {
  mail("agnibindas2021@gmail.com", "Premiumhub message", $message, "from: $name <$email>");
  echo("<script type='text/javascript'>alert(your message sent successfully)</script>");
  window.history.log(-1);
}

?>