# FakeOdbc

A mock Windows [[ODBC]] driver written in C that returns static CSV data regardless of the SQL query sent to it.

**Repo:** `~/Git/FakeOdbc`

FakeOdbc implements the full ODBC 3.x API surface as a Windows DLL, reading a fixed CSV file from a network share and returning it as a three-column result set. Lets applications expecting an ODBC data source be tested without a real database backend. Registers via the Windows Registry as a proper driver with DSN support.
