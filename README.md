<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Leave a Comment</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 20px;
            background-color: #f0f0f0;
        }
        .comment-section {
            max-width: 600px;
            margin: 0 auto;
            background: #fff;
            padding: 20px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        .comment-form {
            display: flex;
            flex-direction: column;
        }
        .comment-form input, .comment-form textarea {
            margin-bottom: 10px;
            padding: 10px;
            font-size: 1em;
            border: 1px solid #ccc;
        }
        .comment-form button {
            padding: 10px 20px;
            background: #007bff;
            color: #fff;
            border: none;
            cursor: pointer;
        }
        .comment-form button:hover {
            background: #0056b3;
        }
        .comments {
            margin-top: 20px;
        }
        .comment {
            background: #f9f9f9;
            padding: 10px;
            border: 1px solid #e0e0e0;
            margin-bottom: 10px;
        }
    </style>
</head>
<body>

<div class="comment-section">
    <h2>Leave a Comment</h2>
    <form class="comment-form" id="commentForm">
        <input type="text" id="name" placeholder="Your Name" required>
        <input type="email" id="email" placeholder="Your Email" required>
        <textarea id="comment" rows="4" placeholder="Your Comment" required></textarea>
        <button type="submit">Submit</button>
    </form>
    <div class="comments" id="comments">
        <h3>Comments</h3>
    </div>
</div>

<script>
    document.getElementById('commentForm').addEventListener('submit', function(event) {
        event.preventDefault();

        // Get form values
        const name = document.getElementById('name').value;
        const comment = document.getElementById('comment').value;

        // Create comment element
        const commentElement = document.createElement('div');
        commentElement.classList.add('comment');
        commentElement.innerHTML = `
            <h4>${name}</h4>
            <p>${comment}</p>
        `;

        // Add comment to comments section
        document.getElementById('comments').appendChild(commentElement);

        // Clear form
        document.getElementById('commentForm').reset();
    });
</script>

</body>
</html>

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Leave a Comment</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 20px;
            background-color: #f0f0f0;
        }
        .comment-section {
            max-width: 600px;
            margin: 0 auto;
            background: #fff;
            padding: 20px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        .comment-form {
            display: flex;
            flex-direction: column;
        }
        .comment-form input, .comment-form textarea {
            margin-bottom: 10px;
            padding: 10px;
            font-size: 1em;
            border: 1px solid #ccc;
        }
        .comment-form button {
            padding: 10px 20px;
            background: #007bff;
            color: #fff;
            border: none;
            cursor: pointer;
        }
        .comment-form button:hover {
            background: #0056b3;
        }
        .comments {
            margin-top: 20px;
        }
        .comment {
            background: #f9f9f9;
            padding: 10px;
            border: 1px solid #e0e0e0;
            margin-bottom: 10px;
        }
    </style>
</head>
<body>

<div class="comment-section">
    <h2>Leave a Comment</h2>
    <form class="comment-form" id="commentForm">
        <input type="text" id="name" placeholder="Your Name" required>
        <input type="email" id="email" placeholder="Your Email" required>
        <textarea id="comment" rows="4" placeholder="Your Comment" required></textarea>
        <button type="submit">Submit</button>
    </form>
    <div class="comments" id="comments">
        <h3>Comments</h3>
    </div>
</div>

<script>
    async function fetchComments() {
        const response = await fetch('http://localhost:3000/comments');
        const comments = await response.json();
        return comments;
    }

    async function postComment(comment) {
        const response = await fetch('http://localhost:3000/comments', {
            method: 'POST',
            headers: {
                'Content-Type': 'application/json'
            },
            body: JSON.stringify(comment)
        });
        return await response.json();
    }

    document.addEventListener('DOMContentLoaded', async function() {
        const commentsContainer = document.getElementById('comments');

        function displayComments(comments) {
            commentsContainer.innerHTML = '<h3>Comments</h3>';
            comments.forEach(comment => {
                const commentElement = document.createElement('div');
                commentElement.classList.add('comment');
                commentElement.innerHTML = `
                    <h4>${comment.name}</h4>
                    <p>${comment.text}</p>
                `;
                commentsContainer.appendChild(commentElement);
            });
        }

        const storedComments = await fetchComments();
        displayComments(storedComments);

        document.getElementById('commentForm').addEventListener('submit', async function(event) {
            event.preventDefault();

            const name = document.getElementById('name').value;
            const commentText = document.getElementById('comment').value;

            const newComment = {
                name: name,
                text: commentText
            };

            await postComment(newComment);

            const updatedComments = await fetchComments();
            displayComments(updatedComments);

            document.getElementById('commentForm').reset();
        });
    });
</script>

</body>
</html>
