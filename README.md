<!DOCTYPE html>
<body>
<div class="final">
        <form>
        <input type="checkbox" name="agree">
        <br>
        <input type="text" name="username" value="tasnim">
        </form>
        <br>
        <form id="searchForm">
            <input type="text" id="searchInput" placeholder="Search...">
            <button type="submit">Search</button>
        </form>
    </div>
    <script>
        document.getElementById('searchForm').addEventListener('submit', function(event) {
            event.preventDefault();
            const query = document.getElementById('searchInput').value.trim().toLowerCase();
            if (query === 'blox') {
                window.location.href = 'https://google.com';
            } else {
                alert('Search term not recognized. Try "blox".');
            }
        });
    </script>
</body>
