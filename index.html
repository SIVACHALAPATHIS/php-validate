<?php
if($_SERVER["REQUEST_METHOD"] == "POST") {
    $name = test_input($_POST["name"]);
    $email = test_input($_POST["email"]);
    $message = test_input($_POST["message"]);

    if(empty($name)) {
        $name_error = "Name is required";
    } else {
        if(!preg_match("/^[a-zA-Z ]*$/",$name)) {
            $name_error = "Only letters and white space allowed";
        }
    }

    if(empty($email)) {
        $email_error = "Email is required";
    } else {
        if(!filter_var($email, FILTER_VALIDATE_EMAIL)) {
            $email_error = "Invalid email format";
        }
    }

    if(empty($message)) {
        $message_error = "Message is required";
    }

    if(empty($name_error) && empty($email_error) && empty($message_error)) {
        $to = "youremail@example.com";
        $subject = "New message from website";
        $body = "Name: $name\nEmail: $email\nMessage: $message";
        $headers = "From: $email";

        if(mail($to, $subject, $body, $headers)) {
            $success_message = "Message sent successfully!";
        } else {
            $error_message = "There was an error sending the message";
        }
    }
}

function test_input($data) {
    $data = trim($data);
    $data = stripslashes($data);
    $data = htmlspecialchars($data);
    return $data;
}
?>
<!DOCTYPE html>
<html>
<head>
    <title>Contact Form</title>
</head>
<body>
    <h1>Contact Us</h1>
    <?php if(!empty($success_message)) { ?>
        <p style="color:green;"><?php echo $success_message; ?></p>
    <?php } ?>
    <?php if(!empty($error_message)) { ?>
        <p style="color:red;"><?php echo $error_message; ?></p>
    <?php } ?>
    <form method="post" action="<?php echo htmlspecialchars($_SERVER["PHP_SELF"]);?>">
        <label>Name:</label>
        <input type="text" name="name" value="<?php echo isset($_POST['name']) ? $_POST['name'] : '' ?>">
        <span style="color:red;"><?php echo isset($name_error) ? $name_error : ''; ?></span>
        <br><br>
        <label>Email:</label>
        <input type="email" name="email" value="<?php echo isset($_POST['email']) ? $_POST['email'] : '' ?>">
        <span style="color:red;"><?php echo isset($email_error) ? $email_error : ''; ?></span>
        <br><br>
        <label>Message:</label>
        <textarea name="message"><?php echo isset($_POST['message']) ? $_POST['message'] : '' ?></textarea>
        <span style="color:red;"><?php echo isset($message_error) ? $message_error : ''; ?></span>
        <br><br>
        <input type="submit" name="submit" value="Submit">
    </form>
</body>
</html>
