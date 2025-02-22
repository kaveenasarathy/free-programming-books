# free-programming-books
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Free Programming Books</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
            padding: 20px;
            background-color: #f4f4f4;
        }
        .book {
            background: white;
            padding: 15px;
            margin: 10px 0;
            border-radius: 5px;
            box-shadow: 2px 2px 10px rgba(0,0,0,0.1);
        }
        .book a {
            text-decoration: none;
            color: blue;
        }
    </style>
</head>
<body>
    <h1>Free Programming Books</h1>
    <div id="book-list"></div>

    <script>
        const books = [
            { title: "JavaScript for Beginners", url: "https://example.com/js-book.pdf" },
            { title: "Python Basics", url: "https://example.com/python-book.pdf" },
            { title: "HTML & CSS Guide", url: "https://example.com/html-css-book.pdf" }
        ];

        const bookList = document.getElementById("book-list");

        books.forEach(book => {
            const bookDiv = document.createElement("div");
            bookDiv.classList.add("book");
            bookDiv.innerHTML = `<h3>${book.title}</h3><a href="${book.url}" target="_blank">Download</a>`;
            bookList.appendChild(bookDiv);
        });
    </script>
</body>
</html>
