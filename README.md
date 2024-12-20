<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Feedback Form</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="feedback-container">
        <h1>Feedback Form</h1>
        <p>We value your feedback! Please fill out the form below.</p>
        <form id="feedbackForm" action="submit_feedback.php" method="POST">
            <!-- Name -->
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" placeholder="Your Name" required>

            <!-- Email -->
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" placeholder="Your Email" required>

            <!-- Rating -->
            <label for="rating">Rating:</label>
            <select id="rating" name="rating" required>
                <option value="">Select Rating</option>
                <option value="5">Excellent</option>
                <option value="4">Good</option>
                <option value="3">Average</option>
                <option value="2">Poor</option>
                <option value="1">Very Poor</option>
            </select>

            <!-- Comments -->
            <label for="comments">Comments:</label>
            <textarea id="comments" name="comments" rows="5" placeholder="Your Comments"></textarea>

            <!-- Submit Button -->
            <button type="submit">Submit Feedback</button>
        </form>
    </div>
    <script src="script.js"></script>
</body>
</html>
