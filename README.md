# splunk-export

utility for exporting large data from splunk instances

## installation / usage

### with npm (recommended)

requires [npm](https://www.npmjs.com/get-npm) to be installed

#### without install (recommended)

```shell script
# run command and follow the instructions
npx splunk-export
````

#### with install

```shell script
# install package
npm install splunk-export

# run command and follow the instructions
splunk-export

````

### as a remote script

```shell script
bash <(curl -s https://raw.githubusercontent.com/specialblend/splunk-export/master/bin/main)
```

## example run

- records: `10,644,392`
- size:`2,215M`
- filename: `splunk-data-2020-02-20-21-34-31.csv`
- time to download:`0:13:58`

```
➜  splunk-export-data git:(master) ✗ npx splunk-export
===== splunk-export =====

splunk-export is a utility for exporting large data from splunk instances

Press any key to continue, or ^C to cancel

I need to gather some information about the target splunk instance.

Enter output filename (default: splunk-data-2020-02-20-21-34-31.csv):
Enter splunk url (default: https://localhost:8089):
Enter splunk index (default: main):
Enter splunk username (default: admin):
Enter splunk password (default: password):

I'm about to connect and export all splunk data with the following settings:

OUTPUT_FILE=splunk-data-2020-02-20-21-34-31.csv

SPLUNK_URL=https://localhost:8089
SPLUNK_INDEX=main
SPLUNK_USERNAME=admin
SPLUNK_PASSWORD=****

Press any key to continue, or ^C to cancel

  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100 2215M    0 2215M    0   118  2704k      0 --:--:--  0:13:58 --:--:--     0
➜  splunk-export-data git:(master) ✗ wc -l splunk-data-2020-02-20-21-34-31.csv
 10644392 splunk-data-2020-02-20-21-34-31.csv
```
