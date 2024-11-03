# CAP Theorem

# CAP

- Consistency
- Availability
- Partition Tolerance

![0ekexbty.bmp](https://raw.githubusercontent.com/hobbes09/BkndEnggMrkTxtResources/main/2024/11/03-08-45-43-uceho11e.png)

![uceho11e.bmp](https://raw.githubusercontent.com/hobbes09/BkndEnggMrkTxtResources/main/2024/11/03-08-45-54-0ekexbty.png)

## Best Video

[https://www.youtube.com/watch?v=KmGy3sU6Xw8](https://www.youtube.com/watch?v=KmGy3sU6Xw8)

# Theory

## Consistency

Whenever we are making any changes in the DB, the same changes should be reflected immediately on any read by same or other process

## Availability

The database is always available for any Read and Write requests.

It does not matter even if it is consistent or not. 

## Partition Tolerance

Partition means that a system of nodes in a DB are not necessarily connected. PT means that the system has the behavior that all the nodes might not be connected by network. 

# System Types

## Consistency - Partition Tolerance

In a master slave architecture, this is the case where the master ensures that any write request is not committed until the same changes in reflected in all slaves. In case it does not happen, then the system is not available. 

## Availability- Partition Tolerance

In a master slave architecture, this is the case where the master processes the write request and commits it, and then not necessarily pushes the same changes for reflection in all slaves. In such cases, the system is not consistent, as replication is async. 

## Consistency - Availability

Single and standalone instance that stores all data in its HDD/SSD. No other systems available.