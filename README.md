### MongoDB Java Driver Configuration
#### serverSelectionTimeout

The server selection timeout in milliseconds, which defines how long the driver will wait for server selection to succeed before throwing an exception.

A value of 0 means that it will timeout immediately if no server is available.  A negative value means to wait indefinitely.

#### connectTimeout

The connection timeout, in milliseconds, which must be greater than 0.

#### socketTimeout

The socket timeout, in milliseconds.

**Suggested:** same as connectTimeout

#### readPreference

The read preference. [Read Preference at MongoDB Manual](https://docs.mongodb.com/manual/core/read-preference/)

**Suggested:** ReadPreference.nearest()

#### readConcern

The read preference. [Read Concern at MongoDB Manual](https://docs.mongodb.com/manual/reference/read-concern/)

##### writeConcern

The write preference. [Write Concern at MongoDB Manual](https://docs.mongodb.com/manual/reference/write-concern/)

**Suggested:** Use the **wtimeout** option to aviod write operation blocking indefinitely
