# Security-Engineering-Week-2-Exercises
Security Engineering-Week 2 Exercises
#Task 1 A:

When a web browser displays a "Not Secure" warning, the website uses an insecure connection, typically HTTP instead of HTTPS. This indicates that any data exchanged between the user's browser and the site is unencrypted.

Risks of Visiting "Not Secure" Sites:
Any personal or financial information (like passwords or credit card details) can be intercepted by attackers. Attackers can modify the data you send. Unsecured sites may be more prone to malware or malicious scripts.
A site is trusted if it has a valid SSL/TLS certificate. The lock symbol or “Secure” label indicates that the connection is encrypted and the site is authenticated.

While the "Not Secure" warning is one indicator, scam sites can sometimes use HTTPS and appear secure. Here are other ways to detect them:
The URL might look similar to a legitimate one but contain typos, extra characters, or a different domain extension.

They are asking for sensitive information outside of expected contexts. Many phishing sites use poorly written content.

Online Tools for Detecting Phishing/Scam Sites : 
Google Safe Browsing: A tool integrated into Chrome and Firefox that alerts users about phishing or malware sites.
PhishTank: A community-driven service where users can report and check phishing websites.
Whois Lookup: Identifies the owner of a domain to help determine whether it’s legitimate or suspicious.

Typosquatting is a form of cybersquatting where attackers register domain names similar to legitimate websites, often with minor typographical errors. For example, a typosquatting site for amazon.com might be amaz0n.com or amzon.com. These fraudulent domains are used to trick users into visiting them, often for phishing, malware distribution, or data theft.

The Uniform Domain-Name Dispute-Resolution Policy (UDRP) is a policy developed by the Internet Corporation for Assigned Names and Numbers to resolve disputes over domain names.

If  I owned ouspg.org and ran my crypto banking application at bank.ouspg.org, I should monitor for similar or misspelt domain names that could be used for phishing. Here are potential domains to watch for:
Common Misspellings: Variations like bnak.ouspg.org, banko.ouspg.org, or b4nk.ouspg.org.
Alternative Domain Extensions: Domains like bankouspg.com, bankouspg.net, or ouspgbank.org.
Homoglyph Attacks: Domains using similar-looking characters, such as replacing "o" with "0" or "g" with "9", like bank.0uspg.org or bank.ouspq.org.
Hyphenated or Extra Characters: Variants like bank-ouspg.org or bankouspg-secure.org.

Task 2 :

Payments:

Modern payment cards use a chip instead of a magnetic stripe because of increased security features and fraud prevention. The chip generates a unique cryptographic code for each transaction. Magnetic stripes store static data that can be easily copied or cloned by skimming devices. Chip cards are much harder to duplicate because of the encryption used in the chip.

An EMV certificate is part of the authentication process that helps ensure the legitimacy of the card and the card issuer during transactions.

EMV uses digital certificates and public/private key encryption to verify that both the card and the terminal are authentic. When you insert the card into a terminal, the chip sends an encrypted message that can only be decrypted with the terminal's public key. EMV certificates prevent man-in-the-middle attacks, where a malicious actor modifies the data exchanged between the card and the terminal.

Despite the added security of EMV chips, payment cards are still susceptible to certain types of attacks:

A skimming device captures the data from the magnetic stripe on the card when it is swiped at an ATM or point-of-sale terminal. A shimmer is a thin, hard-to-detect device inserted into a chip card reader to steal data from chip cards.

Card-not-present fraud occurs when a transaction is made without the physical presence of the card. Cybercriminals trick users into revealing their card details through fake emails or websites. Hackers steal card information from poorly secured databases of online merchants. Malicious code is injected into a website’s checkout page to capture card details when the user purchases. Contactless payment systems are vulnerable to attacks like relay, eavesdropping, and skimming, through encryption.

MFA :

Multi-factor authentication (MFA) is widely used in banking to provide an additional layer of security beyond just a username and password. 

 MFA requires users to present two or more verification factors from different categories before granting access to their accounts or approving transactions. The categories of authentication factors typically used in banking are Something users know (password ), A biometric factor like a fingerprint, facial recognition, or iris scan etc . In banking, MFA is applied in various scenarios like Login Authentication, and Transaction Authorization.

MFA increases payment security by reducing the likelihood of fraud. If an attacker steals a user's password, they would still need access to the second factor (such as a phone or biometric) to complete the authentication process.MFA ensures that only the authorized account holder can confirm transactions.MFA makes it much harder for attackers to succeed even if they trick the user into giving up their password. In daily life, common MFA methods include SMS-Based One-Time Passwords, Authenticator Apps, and Biometrics.

While MFA improves security, certain attacks target different 2FA methods.

Time-Based One-Time Password :

Attackers may trick users into providing their  One-Time Password code by setting up a fake login page. The attacker uses the stolen code before it expires.

Attackers may intercept credentials and the One-Time Password code in real-time, allowing them to authenticate with the stolen information.


Text Message:

Attackers convince the victim's mobile carrier to transfer the phone number to a new SIM card under the attacker’s control. This allows them to receive SMS 2FA codes intended for the victim.
Hackers can exploit vulnerabilities in mobile networks to intercept SMS messages.



Task 3 :



Card fraud can generally be categorized into three types. Card-present fraud occurs when the physical card is stolen or cloned, typically at ATMs or point-of-sale (POS) terminals using techniques like skimming.
Card-not-present fraud happens during online or remote transactions where no physical card is involved. This is increasingly common in e-commerce.
Counterfeit fraud Involves the replication of card data on fake cards, which is most often tied to the use of magnetic stripe technology.

Fraud types vary based on geographical regions. In Europe, card-not-present fraud has become dominant, accounting for 79% of all fraud cases by 2019. The rise of e-commerce in Western Europe, especially in countries like the UK and France, has been accompanied by higher levels of CNP fraud. Conversely, card-present fraud, like skimming, is more prevalent in regions with older technology, particularly areas where EMV chips are not fully adopted.

Between 2008 and 2019, the landscape of card fraud changed significantly. From 2008 to 2011, card-present fraud was more common due to the widespread use of magnetic stripes on cards. However, as EMV chip adoption increased, Card-present fraud decreased significantly. From 2012 onward, Card-not-present fraud surged, driven by the rise in online shopping. By 2019, Card-not-present fraud had become the most dominant form of card fraud, especially as physical card fraud was mitigated by chip and PIN technology.

The most notable increase in fraud between 2008 and 2019 is related to card-not-present transactions. The widespread adoption of e-commerce platforms and mobile payments provided more opportunities for cybercriminals to exploit vulnerable payment systems. This fraud type saw consistent growth over the last decade, overtaking card-present fraud due to increasing online shopping activity.

Several technological advancements and regulatory changes played critical roles in combating fraud during this period:
EMV  chip cards significantly reduced counterfeit fraud. These cards use dynamic authentication, making it more difficult to clone cards compared to the easily replicable magnetic stripe.
 The implementation of the Revised Payment Services Directive  in 2019 introduced Strong Customer Authentication, which required multi-factor authentication for most online transactions. This regulation was crucial in addressing rising CNP fraud.

The years between 2008 and 2019 saw a clear shift from traditional, in-person card transactions to online payments. The number of e-commerce transactions skyrocketed, contributing to the increase in Card-not-present fraud. 

Online or cross-border transactions have historically been associated with higher fraud risks. Card Not Present fraud became especially common in international transactions. As global e-commerce grew, these transactions often involved limited oversight, making them attractive targets for fraudsters. 

The rise of e-commerce was a double-edged sword. While it provided convenience, it also created new opportunities for fraudsters to exploit vulnerabilities in online payment systems. The reliance on traditional password-based authentication was insufficient for many online platforms.

Preventing data breaches became essential in reducing fraud. A significant portion of card-not-present fraud is enabled by breaches that expose sensitive cardholder data, which fraudsters then use to make unauthorized transactions. 

Tokenization has emerged as a key technology to combat card-not-present fraud. By replacing sensitive card details with unique tokens for each transaction, it ensures that even if data is intercepted or stolen, it cannot be used by fraudsters. Tokenization has been especially effective in mobile and contactless payments.

Cross-border fraud has consistently remained a significant portion of card fraud. Many fraud cases involve transactions conducted outside the card issuer’s country.
The decline in card-present fraud reflects the successful implementation of chip-and-PIN technologies and better security at ATMs and POS systems, leading to fewer opportunities for fraudsters to exploit physical cards.
In summary, card fraud evolved significantly between 2008 and 2019. While traditional card-present fraud declined with the adoption of EMV chips and improved regulations grew rapidly due to the rise of e-commerce and online transactions. The focus on securing online transactions through technologies like tokenization and strong customer authentication is likely to shape the future of fraud prevention efforts.



