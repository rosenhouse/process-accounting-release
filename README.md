# bosh release for process accounting

[Process accounting](http://man7.org/linux/man-pages/man5/acct.5.html) is a Linux
kernel feature that tracks running processes and records information about them
to a file on disk.

The `enable` job in this bosh release will enable process accounting.  It
also installs the `acct` package which provides tools like
[`sa`](http://man7.org/linux/man-pages/man8/sa.8.html) and
[`lastcomm`](http://man7.org/linux/man-pages/man1/lastcomm.1.html)
to read the accounting file.

By default, the accounting file lives at `/var/vcap/data/process-accounting/pacct`
