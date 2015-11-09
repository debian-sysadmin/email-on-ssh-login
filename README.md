# email-on-ssh-login
Scripts which will send an eMail after a SSH login event (initialized directly by rsyslogd).

How it works:
0. add the rsyslog config file (from etc/rsyslog.d/ of this repo) into your /etc/rsyslog.d folder.
0. add the host specific config file (from etc/ of this repo somewhere), change the values according to your needs
0. add the binary per file to your /usr/local/sbin/ folder
0. set the path of the host specific config file in the binary
0. restart your rsyslogd daemon