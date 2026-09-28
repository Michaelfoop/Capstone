# Network Vulnerability Scanner
This is my capstone project. It will scan hosts on a network and check softwares on a network against a database of known vulnerabilities, and then make a report of what it found

## Scanner Part

This is the main tool behind it. It needs:
>- It's ability to scan networks (Discover live hosts/ open ports)
>- It's ability to understand the CVE/NVD database
>- It's ability to understand what softwares are on target host and lookup any vulnerabilities

## Target Part

This is what the scanner will be tested against:
>- Virtual Machines (Linux/Windows)
>- Different types of tools/softwares (apache, ssh, nginx, etc.), both outdated and fully updated
I will build a virtual environment for this project, or at the very least, a bunch of different machines on their own

## Possible Addition

After I get the scanner and targets all set up, with numerous types of vulnerable software for it to scan:
>- Well formatted/detailed report (non-tech savvy friendly)
>- Possible web dashboard

---

|Scanner||
|-|-|
|Python|The main language behind the tool|
|Nmap|Network discovery + version detection|
|python-nmap|let's the code run nmap/read its results|
|requests|python library that will make requests to the database|
|NVD API/key|For the code to reach the CVEs|

|Report||
|-|-|
|Jinja2|Fills in an HTML report template with our scan data|
|WeasyPrint or ReportLab|Turns the HTML template into a pdf|

The VMs I'll need are the following:
>- Windows User
>- Linux User
>- Linux Server
>- Metasploitable2 (linux vm designed to have security holes)
