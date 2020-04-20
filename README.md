# Nginx bootcamp
> Summary for basic Nginx

```
  # Basic command

    - set $<variable> <value>
    - location = /<uri>         : 
    - location ~ /<uri>         : Case sensitive with uri
    - location ~* /<uri>        : Case insensitive with uri
    - location ~ /<uri>[0-9]    : Regular expression  
    - rewrite /<original-uri>/ <to-uri>
    - rewrite /<original-uri>/(regex) <to-uri>?<queryStr>
    - try_files
    - access_log
    - access_error
    - worker_processes 4
    - worker_connection 1024
    - client_body_buffer_size 40k;
    - client_max_body_size 10m;
    - client_header_buffer_size 1k;

      ## Timeout ##
    Max time to receive headers/body (second)
    - client_body_timeout 12
    - client_header_timeout 12

    Max to keep a connection open for
    - keepalive_timeout 15

    Max connections to keep a connection open for
    - keepalive_requests 1024

    Max for the client accept/receive a response
    - send_timeout 10
```

- License: MIT
- Author: Kraipon Najaroon