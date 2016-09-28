# passmg
Password manager for shared secrets using GPG for encryption and authentication.

       passmg is a perl script designed to lessen the problems of shared/common passwords amongst administators.  Although having passwords being used by multiple individuals is
       itself a risk, especially when auditing actions performed using that password, it is often an inescapable nessessity.  This problem is further aggrevated by a tendency to change
       shared passwords very infrequently due largly to the difficulties involved in diseminating the new passwords to all parties in a way that does not itself further compromise it.

       passmg addresses this problem by keeping a central repository of passwords stored in PGP encrypted files.  Each user who has been granted access to the repository has their own PGP
       public and private key pair.  Each password file is encrypted using all the appropriate public keys meaning each user can access the respository using their own pass phrase.  Access
       control is determined username and group membership on a per key basis.
