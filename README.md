# Railway Reservation System (Java Console Project)

A backend-only Java console application for train search, seat availability, reservations, PNR lookup, cancellation, and FIFO waiting-list promotion.

## Requirements
- Java 17 or newer (Java 21 recommended)
- No database, GUI, frontend, or external libraries

## Run
From the project root:

```bash
 javac -d out $(find src/main/java -name "*.java")
 java -cp out app.Main
```

On Windows PowerShell, compile with:

```powershell
$files = Get-ChildItem -Recurse src/main/java -Filter *.java | ForEach-Object { $_.FullName }
javac -d out $files
java -cp out app.Main
```

All data is stored in memory and resets when the application exits.
