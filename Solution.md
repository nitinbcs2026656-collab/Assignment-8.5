```html
<!DOCTYPE html>
<html>
<head>
    <title>Photo Gallery</title>
    <style>
        * {
            box-sizing: border-box;
        }

        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background: #f1f5f9;
        }

        .container {
            display: grid;
            grid-template-columns: 1fr;
            grid-template-areas:
                "header"
                "gallery"
                "footer";
            gap: 20px;
            padding: 20px;
        }

        header {
            grid-area: header;
            background: #1e293b;
            color: white;
            text-align: center;
            padding: 20px;
        }

        .gallery {
            grid-area: gallery;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 20px;
        }

        .card {
            background: white;
            border-radius: 10px;
            overflow: hidden;
        }

        .card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            display: block;
        }

        .card h3 {
            padding: 0 15px;
            overflow-wrap: anywhere;
        }

        .card p {
            padding: 0 15px 15px;
            color: #475569;
            overflow-wrap: anywhere;
        }

        footer {
            grid-area: footer;
            background: #1e293b;
            color: white;
            text-align: center;
            padding: 15px;
        }
    </style>
</head>
<body>

<div class="container">
    <header>
        <h1>My Photo Gallery</h1>
        <p>Explore Beautiful Places</p>
    </header>

    <main class="gallery">
        <div class="card">
            <img src="https://picsum.photos/id/10/400/300" alt="Forest">
            <h3>Green Forest</h3>
            <p>Enjoy the beauty of nature.</p>
        </div>

        <div class="card">
            <img src="https://picsum.photos/id/29/400/300" alt="Mountain">
            <h3>Mountains</h3>
            <p>Discover amazing mountain views.</p>
        </div>

        <div class="card">
            <img src="https://picsum.photos/id/37/400/300" alt="Sea">
            <h3>Beautiful Sea</h3>
            <p>Relax beside the ocean.</p>
        </div>

        <div class="card">
            <img src="https://picsum.photos/id/42/400/300" alt="Nature">
            <h3>Nature</h3>
            <p>Experience peaceful surroundings.</p>
        </div>

        <div class="card">
            <img src="https://picsum.photos/id/57/400/300" alt="Travel">
            <h3>Travel</h3>
            <p>Explore new destinations.</p>
        </div>

        <div class="card">
            <img src="https://picsum.photos/id/65/400/300" alt="City">
            <h3>City Life</h3>
            <p>Discover the beauty of cities.</p>
        </div>
    </main>

    <footer>
        <p>© 2026 My Photo Gallery</p>
    </footer>
</div>

</body>
</html>
```