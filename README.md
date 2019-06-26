# Syscache Parser

Syscache Parser is a quick script designed to parse the SHA1 hashes from Syscache.hve into a CSV file. 

I often find myself identifying Syscache artifacts during disk timelining, and parsing them manually is cumbersome. With Syscache Parser, the goal is to pivot on timestamps of interest, and then look up hashes accordingly. 

## Installation 

I have provided an executable which can be used to parse Syscache.hve. You can also use the Python version by installing the dependencies specified in requirements.txt:

```bash
pip3 install -r requirements.txt
```

## Usage

Syscache Parser takes the following arguments:

* -f syscache.hve
	* Syscache Hive to parse (required)
* -o output.csv
	* File to save results to (required)
* -n hostname
	* Hostname of system (optional) 

```bash
syscache.exe -f syscache.hve -o output.csv -n hostname
```

```python
python3 syscache.py -f syscache.hve -o output.csv -n hostname
```

