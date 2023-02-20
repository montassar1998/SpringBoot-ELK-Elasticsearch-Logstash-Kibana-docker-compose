if you want to send multiple requests to test this

`xargs -I % -P 10 curl -I "172.22.224.1:8080" < <(printf '%s\n' {1..10})`

change to the number of queries you want to have 