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

- records: `5,650,032`
- size:`562M`
- filename: `splunk-data-2020-02-21-00-08-00.log`
- time to download:`0:01:58`

```
➜  splunk-data-export npx splunk-export
===== splunk-export =====

splunk-export is a utility for exporting large data from splunk instances

Press any key to continue, or ^C to cancel

I need to gather some information about the target splunk instance.

Enter output filename (default: splunk-data-2020-02-21-00-08-00.log):
Enter splunk url (default: https://localhost:8089):
Enter splunk index (default: main):
Enter splunk username (default: admin):
Enter splunk password (default: password):

I'm about to connect and export all splunk data with the following settings:

OUTPUT_FILE=splunk-data-2020-02-21-00-08-00.log

SPLUNK_URL=https://localhost:8089
SPLUNK_INDEX=main
SPLUNK_USERNAME=admin
SPLUNK_PASSWORD=****

Press any key to continue, or ^C to cancel

  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100  562M    0  562M  100   118  7639k      1  0:01:58  0:01:15  0:00:43     0
➜  splunk-data-export wc -l splunk-data-2020-02-21-00-08-00.log
 5650032 splunk-data-2020-02-21-00-08-00.log

```
