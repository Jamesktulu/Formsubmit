<!DOCTYPE html>
<html>
<head>
	<title>Contact Form</title>
	<script>
		function submitForm() {
			// Get form data
			let name = document.getElementById("name").value;
			let email = document.getElementById("email").value;
			let message = document.getElementById("message").value;

			// Validate form data (for example, check that name and email are not empty)

			// Display thank you message
			document.getElementById("form").style.display = "none";
			document.getElementById("thankyou").style.display = "block";
		}
	</script>
	<style>
		#thankyou {
			display: none;
		}
	</style>
</head>
<body>
	<h1>Contact Us</h1>
	<form id="form" class="exs-ajax-form" action="https://formsubmit.co/hope-everywhere@mail.com" method="POST">
		<label for="name">Name:</label>
		<input required="required" placeholder="Enter your name" name="name" type="text" id="name" class="d-block mb-1">

		<label for="email">Email:</label>
		<input required="required" placeholder="Enter your email address" name="email" type="email" id="email" class="d-block mb-1">

		<label for="message">Message:</label>
		<textarea required="required" placeholder="Enter your message" name="message" id="message" class="d-block mb-1"></textarea>

		<button type="submit" onclick="submitForm()">Submit</button>
	</form>
	<div id="thankyou">
		<p>Thank you for contacting us, we will get back to you as soon as possible.</p>
	</div>
</body>
</html>
