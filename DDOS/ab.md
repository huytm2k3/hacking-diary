## Using ab for DDOS

```bash
ab -n 10000 -c 100 http://example.com/
```

- `-n`: Number of requests
- `-c`: Number of concurrent requests

Oh I just tried it on static website, and I htop on that server (16GB RAM and 12 CPU). All cores of CPU are fluctuates from 50% to 70%.

If I try to DDOS on some endpoints with heavy tasks, that server maybe down.