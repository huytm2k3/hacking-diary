## Using sqlmap for SQL injection

### Getting HTTP raw from browser
Because sqlmap need HTTP raw to inject, we need to get it from browser.
- Step 1: Open devtools in browser (F12)
- Step 2: Process the request and follow it in Network tab
- Step 3: Right click on the request and click "Copy" -> "Copy as cURL"
- Step 4: Open https://curlconverter.com/http/ and paste the cURL
- Step 5: Copy the HTTP raw and paste it to sqlmap

### Injecting
```bash
sqlmap -r http_raw.txt --batch
```

- `--batch`: Run sqlmap in batch mode
- `-r`: Read HTTP raw from file
