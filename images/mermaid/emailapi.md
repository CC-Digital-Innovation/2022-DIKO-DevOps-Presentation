graph TD
    A[API Data] -->|Files and email data| C{EmailAPI}
    C -->|Html tabular report| D[Email Server]
    C -->|logs| E[Syslog Server]
    C -->|files and email data| F[Noco Database]