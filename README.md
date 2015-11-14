## email-or-xmpp-message-on-ssh-login
Scripts which will send an eMail or an xmpp message after a SSH login event (initialized directly by rsyslogd).

How it works:
* put the rsyslog config file (from etc/rsyslog.d/ of this repo) into your /etc/rsyslog.d folder.
* put the host specific config file (from etc/ of this repo) somewhere, change the values according to your needs, also take care of changing the last HOSTNAME part to fit the hostname of your system
* put the binary per file to your /usr/local/sbin/ folder
* set the path of the host specific config file in the binary, pay attention to specify the absolute path
* restart your rsyslogd daemon
