# racoon assumes the presence of the kernel random number device rnd(4) at
 ##     /dev/urandom.

### RETURN VALUES
     The command exits with 0 on success, and non-zero on errors.

### FILES
     /private/etc/racoon/racoon.conf       default configuration file.
     /private/etc/racoon/psk.txt           default pre-shared key file.

SEE ALSO
     ipsec(4), racoon.conf(5), syslog.conf(5), setkey(8), syslogd(8)

HISTORY
     The racoon command first appeared in the ``YIPS'' Yokogawa IPsec imple-
     mentation.

SECURITY CONSIDERATIONS
     The use of IKE phase 1 aggressive mode is not recommended, as described
     in http://www.kb.cert.org/vuls/id/886601.
