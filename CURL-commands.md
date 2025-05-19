List of the most useful curl commands!

🎯 Most Useful curl Commands for Downloading and Interacting with URLs  
(With Emoji for Better Understanding)  

# 1️⃣ Basic GET Request  
Use curl to fetch the content of a URL.  
curl https://example.com

# 2️⃣ Save to a File  
Use -o to save the downloaded content to a file.  
curl -o filename.html https://example.com

# 3️⃣ Display Response Headers  
Use -I to only fetch the response headers.  
curl -I https://example.com

# 4️⃣ Follow Redirects  
Use -L to follow redirects (if the URL redirects you).  
curl -L https://example.com

# 5️⃣ Download a File (with Resume)  
Use -C to resume a partially downloaded file.  
curl -C - -O https://example.com/largefile.zip

# 6️⃣ Show Progress  
Use -# to show a progress bar during download.  
curl -# -O https://example.com/largefile.zip

# 7️⃣ Download a Torrent  
Use -o to download and save a .torrent file.  
curl -o ubuntu-22.04.iso.torrent https://releases.ubuntu.com/22.04/ubuntu-22.04.5-live-server-amd64.iso.torrent

# 8️⃣ Send a POST Request  
Use -X POST to send data to a server (e.g., form submission).  
curl -X POST -d "username=user&password=pass" https://example.com/login

# 9️⃣ Include Custom Headers  
Use -H to add custom headers to your request.  
curl -H "Authorization: Bearer TOKEN" https://api.example.com/data

# 🔟 Make a PUT Request  
Use -X PUT to send data to update a resource.  
curl -X PUT -d '{"name": "John"}' -H "Content-Type: application/json" https://example.com/update

# 🔒 Send Data with Authentication  
Use -u to pass authentication credentials.  
curl -u username:password https://example.com

# 1️⃣1️⃣ Save Cookies  
Use -c to save cookies to a file.  
curl -c cookies.txt https://example.com

# 1️⃣2️⃣ Use Cookies from a File  
Use -b to send cookies from a saved file.  
curl -b cookies.txt https://example.com

# 1️⃣3️⃣ Limit Download Speed  
Use --limit-rate to limit download speed.  
curl --limit-rate 100K -O https://example.com/largefile.zip

# 1️⃣4️⃣ Show Full Request & Response  
Use -v for verbose output (request and response details).  
curl -v https://example.com

# 1️⃣5️⃣ Send Data as JSON  
Use -H and -d to send data as JSON.  
curl -X POST -H "Content-Type: application/json" -d '{"key": "value"}' https://example.com/api

# 1️⃣6️⃣ Access a URL with SSL Verification Disabled  
Use -k or --insecure to skip SSL certificate verification (not recommended for production).  
curl -k https://example.com

# 1️⃣7️⃣ Limit Request Time  
Use --max-time to limit the total request time.  
curl --max-time 10 https://example.com

# 1️⃣8️⃣ Download Multiple Files  
Use -O to download multiple files at once.  
curl -O https://example.com/file1.zip -O https://example.com/file2.zip

# 1️⃣9️⃣ Get Information About the URL  
Use -I to fetch only headers for a URL.  
curl -I https://example.com

# 2️⃣0️⃣ Use a Proxy  
Use -x to route your request through a proxy.  
curl -x proxy.example.com:8080 https://example.com
