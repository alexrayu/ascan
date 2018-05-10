# aScan PHP Code Scanner

Scans the code for signatures of hacks. Use it for recently hacked sites.

The script will scan for recently created php files (< 7 days old) and php files matching hack patterns.

The srcipt file will create an output called suspicious.csv, listing possible threats.

Originally developer for [InDigiMar](https://indigimar.com).

## Usage

1. Put the script file in a folder which you want to scan recursively. Usually, it's the web site's root folder.
2. Set the script an executable byte (give permission to execute).
3. Call the command like this: ./ascan.
4. The output will show how many suspicious files have been found.
5. Open the suspicious.csv file and see the list of files and matches against which they gave positives. 
6. Verify the suspected files manually. Delete or edit the confirmed positives.
7. Remove the script. Don't leave it around, as it contains threat patterns and can itself become source of alerts with some hostings.