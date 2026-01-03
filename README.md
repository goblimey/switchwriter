# SwitchWriter

A managed go writer

The switch writer is a managed io.Writer written in Go.
It provides a destination stream that can be changed dynamically. 
The destination stream can be switched to another file.
It can also be disabled altogether, in which case all writes to it are silently discarded,
and then re-enabled.

The switch writer demo shows how it can be used.
It's used as part of my daily logger,
a SLOG solution that writes to a log file.
The log file rolls over to a new version each day.

The SwitchWriter was written by my friend and colleague Mark Rafter.
