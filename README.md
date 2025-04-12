## Script: Enable Automatic Seeding Compression (Trace Flag 9567)

**Description**:
This script enables SQL Server trace flag `9567` globally, which activates **compression for automatic seeding** in Always On Availability Groups. This can help reduce the time and network bandwidth required during seeding operations.

**Commands**:
- `DBCC TRACEON (9567, -1)`: Enables trace flag 9567 globally.
- `DBCC TRACESTATUS (9567, -1)`: Confirms whether the trace flag is active.

**Use Case**:
Use this when setting up or optimizing Always On AGs, especially in bandwidth-sensitive environments.

**Requirements**:
- SQL Server 2016 SP1 CU2 or later
- sysadmin privileges
