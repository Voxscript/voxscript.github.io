<h1>Exclusive Early Access to Voxscript</h1>
<p>Join us in shaping Voxscript! Your participation in our early access program grants you unlimited access to Voxscript features for MS Teams, along with the unique opportunity to engage directly with our development team while allowing us to build the plugin that you want to use.</p>
<p>You're free to opt-out whenever you choose. All early access fees are reinvested into supporting the external services that power Voxscript.</p>
<p><b><a id="offer-link" href="#">Subscribe via Stripe</a></b></p>
<br/>
<p>
 Looking for organizational pricing? Drop us <a href="mailto:voxscript@allwiretech.com">line</a> and more to be announced soon!
</p>

<script>
         window.onload = function() {
             // Function to get URL parameters
             function getParameterByName(name, url = window.location.href) {
                 name = name.replace(/[\[\]]/g, '\\$&');
                 var regex = new RegExp('[?&]' + name + '(=([^&#]*)|&|#|$)'),
                     results = regex.exec(url);
                 if (!results) return null;
                 if (!results[2]) return '';
                 return decodeURIComponent(results[2].replace(/\+/g, ' '));
             }
 
             // Get the 'url' parameter
             var encodedUrl = getParameterByName('url');
 
             // Check if the 'url' parameter exists
             if (encodedUrl) {
                 // Decode the URL
                var decodedUrl = decodeURIComponent(encodedUrl);
                document.getElementById('offer-link').href = decodedUrl;
                document.getElementById('offer-box').style.display = 'block';
 
                 // Redirect to the URL
                 //window.location.href = decodedUrl;
             } else {
                 // If no URL is provided, you can redirect to a default page or show an error
                 console.log('No URL provided');
             }
         };
</script>

