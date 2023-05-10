<!DOCTYPE html>
<html>
<head>
	<title>Random Quote Generator</title>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>
	<h1>Random Quote Generator</h1>
	<p>Click the button to generate a random quote:</p>
	<button onclick="generateQuote()">Generate</button>
	<p id="result"></p>

	<script>
		function generateQuote() {
			var quotes = [
				"Be the change you wish to see in the world. - Mahatma Gandhi",
				"The only way to do great work is to love what you do. - Steve Jobs",
				"I have not failed. I've just found 10,000 ways that won't work. - Thomas Edison",
				"Believe you can and you're halfway there. - Theodore Roosevelt",
				"Success is not final, failure is not fatal: It is the courage to continue that counts. - Winston Churchill"
			];
			var quote = quotes[Math.floor(Math.random() * quotes.length)];
			document.getElementById("result").innerHTML = quote;
		}
	</script>
</body>
</html>
