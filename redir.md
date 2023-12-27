    <style>
        .offer-box {
            border: 2px solid #4CAF50;
            border-radius: 5px;
            padding: 20px;
            margin: 20px;
            text-align: center;
            background-color: #f2f2f2;
        }

        .offer-box a {
            color: #4CAF50;
            font-weight: bold;
            text-decoration: none;
        }

        .offer-box a:hover {
            text-decoration: underline;
        }
    </style>
  
     <div id="offer-box" class="offer-box" style="display:none;">
        <h2>Voxscript Early Access Offer</h2>
        <p>Exclusive access just a click away!</p>
        <a id="offer-link" href="#">Access Now</a>
    </div>
    
    <script>
        window.onload = function() {
            function getParameterByName(name, url = window.location.href) {
                name = name.replace(/[\[\]]/g, '\\$&');
                var regex = new RegExp('[?&]' + name + '(=([^&#]*)|&|#|$)'),
                    results = regex.exec(url);
                if (!results) return null;
                if (!results[2]) return '';
                return decodeURIComponent(results[2].replace(/\+/g, ' '));
            }

            var encodedUrl = getParameterByName('url');
            if (encodedUrl) {
                var decodedUrl = decodeURIComponent(encodedUrl);
                document.getElementById('offer-link').href = decodedUrl;
                document.getElementById('offer-box').style.display = 'block';
            } else {
                console.log('No URL provided');
            }
        };
    </script>
