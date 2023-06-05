# Chapter: Directory and File Discovery with GoBuster

## Section 1: GoBuster - Definition and Purpose

GoBuster is a robust open-source utility written in the Go language. Its primary use is in cyber security, particularly for brute-forcing Uniform Resource Identifiers (URIs), including directories and files in websites, DNS subdomains, and Virtual Host names on target web servers. Developed with penetration testers in mind, GoBuster aids in the enumeration process, uncovering "hidden" directories and files on a web server that may not be linked from the publicly accessible part of the application.

## Section 2: When and Why to Use GoBuster

GoBuster is typically employed during the reconnaissance phase of an ethical hacking or penetration testing operation. The following scenarios offer insight into when using GoBuster can be particularly beneficial:

1. **Uncovering Hidden Directories and Files**: GoBuster can identify directories and files that aren't linked from the website's homepage or are otherwise invisible to standard users.

2. **DNS Enumeration**: GoBuster can enumerate subdomains of a target domain, potentially revealing additional attack vectors.

3. **Virtual Hosts Discovery**: For servers hosting multiple websites, GoBuster can identify these virtual hosts, each potentially bearing unique vulnerabilities.

By leveraging GoBuster, it becomes possible to identify additional attack vectors that might not be immediately visible from regular interaction with the application through a web browser. This makes GoBuster an indispensable tool in the repertoire of every ethical hacker.

## Section 3: Top 10 Popular GoBuster Commands

Note: Replace "[target]" with your actual target.

1. **Directory/File Bruteforcing**:
   ```
   gobuster dir -u http://[target] -w /usr/share/wordlists/dirb/common.txt
   ```
   This command attempts to bruteforce directories and files on a website using a predefined wordlist.

2. **DNS Subdomain Enumeration**:
   ```
   gobuster dns -d [target] -w /usr/share/wordlists/SecLists/Discovery/DNS/subdomains-top1million-5000.txt
   ```
   This command serves to enumerate DNS subdomains using a given wordlist.

3. **Virtual Host Enumeration**:
   ```
   gobuster vhost -u http://[target] -w /usr/share/wordlists/SecLists/Discovery/Web-Content/common.txt
   ```
   This command is useful for enumerating virtual hosts using a specified wordlist.

4. **Using Specific HTTP Methods**:
   ```
   gobuster dir -u http://[target] -w /usr/share/wordlists/dirb/common.txt -m POST
   ```
   This command allows you to make POST requests to the target during the bruteforce attack.

5. **Setting HTTP Headers**:
   ```
   gobuster dir -u http://[target] -w /usr/share/wordlists/dirb/common.txt -H "Authorization: Bearer [Token]"
   ```
   This command enables the addition of a specific HTTP header to the requests.

6. **Adding Username and Password**:
   ```
   gobuster dir -u http://[target] -w /usr/share/wordlists/dirb/common.txt -U admin -P password
   ```
   This command adds Basic HTTP Authentication credentials to the requests.

7. **Adding Cookies**:
   ```
   gobuster dir -u http://[target] -w /usr/share/wordlists/dirb/common.txt -c "sessionid=[cookie]"
   ```
   This command adds a specific cookie to the requests.

8. **Setting User Agent**:
   ```
   gobuster dir -u http://[target] -w /usr/share/wordlists/dirb/common.txt -a "Mozilla/5.0"
   ```
   This command modifies the User-Agent in the HTTP request headers.

9. **Ignoring SSL Certificate**:
   ```
   gobuster dir -k -u https://[target] -w /usr/share/wordlists/dirb/common.txt
   ```
   This command tells GoBuster to ignore SSL certificate verification.

10. **Setting a Timeout Limit**:
    ```
    gobuster dir -u http://[target] -w /usr/share/wordlists/dirb/common.txt -t 100
    ```
    This command sets a timeout limit for HTTP requests.

It's important to remember to use tools like GoBuster responsibly and only when you have the appropriate permissions to perform penetration testing activities.
