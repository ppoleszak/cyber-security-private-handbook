# Hashcat - Password Cracking Tool

## 1. Definition and Functionality of Hashcat

Hashcat is a password cracking tool extensively used in the cybersecurity world. It is employed by penetration testers, system administrators, and unfortunately, also by cybercriminals.

Hashcat serves to crack complex passwords stored in the form of so-called hashes, i.e., the encrypted form of a password. With its advanced algorithms, it's capable of "reversing" the encryption process and recovering the original password from the hash, which is crucial in many aspects of network security.

## 2. When to Use Hashcat

Hashcat can be used in various situations, including:

- **Password Security Checks**: System administrators can use Hashcat to test the strength of user passwords. If Hashcat can easily crack a password, so can a potential attacker.

- **Penetration Testing**: Hashcat is often used during penetration testing to crack passwords and gain access to protected systems.

Always remember that this tool should be used responsibly and always in accordance with the law.

## 3. Top 10 Most Commonly Used Hashcat Commands

1. **Dictionary Attack**: `hashcat -m 0 -a 0 hash.txt wordlist.txt`
    - This example shows a simple dictionary attack.

2. **Combinator Attack**: `hashcat -m 0 -a 1 hash.txt wordlist1.txt wordlist2.txt`
    - This example shows a combinator attack that combines words from two different wordlists.

3. **Mask Attack**: `hashcat -m 0 -a 3 hash.txt ?l?l?l?l?l?l?l?l?l`
    - This example shows a mask attack which is highly effective if we know the structure of the password.

4. **Rule-Based Attack**: `hashcat -m 0 -a 0 -r rules/best64.rule hash.txt wordlist.txt`
    - This example shows a rule-based attack which is one of the most complicated attack modes.

5. **Brute Force Attack**: `hashcat -m 0 -a 3 hash.txt ?a?a?a?a?a?a?a?a`
    - This example shows a brute-force attack that tries all possible combinations.

6. **WPA/WPA2 Passwords Attack**: `hashcat -m 2500 -a 0 capture.hccapx wordlist.txt`
    - This example shows how to attack WPA/WPA2 passwords using hashcat.

7. **Hybrid Wordlist + Mask Attack**: `hashcat -m 0 -a 6 hash.txt wordlist.txt ?d?d?d?d`
    - This example shows how to perform a hybrid attack that enables faster password recovery.

8. **Combination Attack**: `hashcat -m 0 -a 1 hash.txt wordlist.txt`
    - This example shows how you can combine different attack methods to increase effectiveness.

9. **Hybrid Attack**: `hashcat -m 0 -a 6 hash.txt wordlist.txt ?d?d?d?d`
    - This example shows how to perform a hybrid attack that combines dictionary attack with mask attack.

10. **Hash Cracking**: `hashcat -m 1000 -a 0 -o cracked.txt hash.txt wordlist.txt`
    - This example shows how to reverse a hash, i.e., an encrypted password, back to its original form.
