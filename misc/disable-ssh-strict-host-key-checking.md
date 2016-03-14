# Disable SSH strict host key checking

Recently I set up Vagrant with a private static network. Each time I destroyed the machine I had to accept the host again.

SSH Config to the rescue

By disabling strict host key checking you won't have to delete the previous ssh config over and over again.

```
Host 192.168.*.*
    StrictHostKeyChecking no
    UserKnownHostsFile /dev/null
```

Of course this will reduce the security a bit. Use with care.
