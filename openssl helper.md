Last login: Wed Oct  9 16:01:04 on ttys001
bob ~ $ open server.key     
bob ~ $ gpg --fingerprint
bob ~ $ gpg
_______
“quick |
 start_|
/\        {=_= } “hm, wtf is gpg?” “well it says for beginners, let’s try”

 
Last login: Wed Oct 1938 16:01:04 on ttys001


blimp@weareribbitpmmes-MacBook-Pro ~ % open server.key     
blimp@weareribbitpmmes-MacBook-Pro ~ % gpg --fingerprint
zsh: command not found: gpg
bob ~ $ openssl help          
openssl:Error: 'help' is an invalid command.

- 

Standard commands
asn1parse         ca                certhash          ciphers           
crl               crl2pkcs7         dgst              dh                
dhparam           dsa               dsaparam          ec                
ecparam           enc               errstr            gendh             
gendsa            genpkey           genrsa            nseq              
ocsp              passwd            pkcs12            pkcs7             
pkcs8             pkey              pkeyparam         pkeyutl           
prime             rand              req               rsa               
rsautl            s_client          s_server          s_time            
sess_id           smime             speed             spkac             
ts                verify            version           x509              

Message Digest commands (see the `dgst' command for more details)
gost-mac          md4               md5               md_gost94         
ripemd160         sha1              sha224            sha256            
sha384            sha512            streebog256       streebog512       
whirlpool         

Cipher commands (see the `enc' command for more details)
aes-128-cbc       aes-128-ecb       aes-192-cbc       aes-192-ecb       
aes-256-cbc       aes-256-ecb       base64            bf                
bf-cbc            bf-cfb            bf-ecb            bf-ofb            
camellia-128-cbc  camellia-128-ecb  camellia-192-cbc  camellia-192-ecb  
camellia-256-cbc  camellia-256-ecb  cast              cast-cbc          
cast5-cbc         cast5-cfb         cast5-ecb         cast5-ofb         
chacha            des               des-cbc           des-cfb           
des-ecb           des-ede           des-ede-cbc       des-ede-cfb       
des-ede-ofb       des-ede3          des-ede3-cbc      des-ede3-cfb      
des-ede3-ofb      des-ofb           des3              desx              
rc2               rc2-40-cbc        rc2-64-cbc        rc2-cbc           
rc2-cfb           rc2-ecb           rc2-ofb           rc4               
rc4-40            

blimp@weareribbitpmmes-MacBook-Pro ~ % openssl enc
aes-128-cbc     
?
aes-128-cbc
?
blimp@weareribbitpmmes-MacBook-Pro ~ % openssl enc -V
usage: enc -ciphername [-AadePp] [-base64] [-bufsize number] [-debug]
    [-in file] [-iv IV] [-K key] [-k password]
    [-kfile file] [-md digest] [-none] [-nopad] [-nosalt]
    [-out file] [-pass arg] [-S salt] [-salt]

 -A                 Process base64 data on one line (requires -a)
 -a                 Perform base64 encoding/decoding (alias -base64)
 -bufsize size      Specify the buffer size to use for I/O
 -d                 Decrypt the input data
 -debug             Print debugging information
 -e                 Encrypt the input data (default)
 -in file           Input file to read from (default stdin)
 -iv IV             IV to use, specified as a hexadecimal string
 -K key             Key to use, specified as a hexadecimal string
 -md digest         Digest to use to create a key from the passphrase
 -none              Use NULL cipher (no encryption or decryption)
 -nopad             Disable standard block padding
 -out file          Output file to write to (default stdout)
 -P                 Print out the salt, key and IV used, then exit
                      (no encryption or decryption is performed)
 -p                 Print out the salt, key and IV used
 -pass source       Password source
 -S salt            Salt to use, specified as a hexadecimal string
 -salt              Use a salt in the key derivation routines (default)
 -v                 Verbose

Valid ciphername values:

 -aes-128-cbc              -aes-128-cbc-hmac-sha1    -aes-128-cfb             
 -aes-128-cfb1             -aes-128-cfb8             -aes-128-ctr             
 -aes-128-ecb              -aes-128-gcm              -aes-128-ofb             
 -aes-128-xts              -aes-192-cbc              -aes-192-cfb             
 -aes-192-cfb1             -aes-192-cfb8             -aes-192-ctr             
 -aes-192-ecb              -aes-192-gcm              -aes-192-ofb             
 -aes-256-cbc              -aes-256-cbc-hmac-sha1    -aes-256-cfb             
 -aes-256-cfb1             -aes-256-cfb8             -aes-256-ctr             
 -aes-256-ecb              -aes-256-gcm              -aes-256-ofb             
 -aes-256-xts              -aes128                   -aes192                  
 -aes256                   -bf                       -bf-cbc                  
 -bf-cfb                   -bf-ecb                   -bf-ofb                  
 -blowfish                 -camellia-128-cbc         -camellia-128-cfb        
 -camellia-128-cfb1        -camellia-128-cfb8        -camellia-128-ecb        
 -camellia-128-ofb         -camellia-192-cbc         -camellia-192-cfb        
 -camellia-192-cfb1        -camellia-192-cfb8        -camellia-192-ecb        
 -camellia-192-ofb         -camellia-256-cbc         -camellia-256-cfb        
 -camellia-256-cfb1        -camellia-256-cfb8        -camellia-256-ecb        
 -camellia-256-ofb         -camellia128              -camellia192             
 -camellia256              -cast                     -cast-cbc                
 -cast5-cbc                -cast5-cfb                -cast5-ecb               
 -cast5-ofb                -chacha                   -des                     
 -des-cbc                  -des-cfb                  -des-cfb1                
 -des-cfb8                 -des-ecb                  -des-ede                 
 -des-ede-cbc              -des-ede-cfb              -des-ede-ofb             
 -des-ede3                 -des-ede3-cbc             -des-ede3-cfb            
 -des-ede3-cfb1            -des-ede3-cfb8            -des-ede3-ofb            
 -des-ofb                  -des3                     -desx                    
 -desx-cbc                 -gost89                   -gost89-cnt              
 -gost89-ecb               -id-aes128-GCM            -id-aes192-GCM           
 -id-aes256-GCM            -rc2                      -rc2-40-cbc              
 -rc2-64-cbc               -rc2-cbc                  -rc2-cfb                 
 -rc2-ecb                  -rc2-ofb                  -rc4                     
 -rc4-40                   -rc4-hmac-md5            
blimp@weareribbitpmmes-MacBook-Pro ~ % openssl server
openssl:Error: 'server' is an invalid command.

Standard commands
asn1parse         ca                certhash          ciphers           
crl               crl2pkcs7         dgst              dh                
dhparam           dsa               dsaparam          ec                
ecparam           enc               errstr            gendh             
gendsa            genpkey           genrsa            nseq              
ocsp              passwd            pkcs12            pkcs7             
pkcs8             pkey              pkeyparam         pkeyutl           
prime             rand              req               rsa               
rsautl            s_client          s_server          s_time            
sess_id           smime             speed             spkac             
ts                verify            version           x509              

Message Digest commands (see the `dgst' command for more details)
gost-mac          md4               md5               md_gost94         
ripemd160         sha1              sha224            sha256            
sha384            sha512            streebog256       streebog512       
whirlpool         

Cipher commands (see the `enc' command for more details)
aes-128-cbc       aes-128-ecb       aes-192-cbc       aes-192-ecb       
aes-256-cbc       aes-256-ecb       base64            bf                
bf-cbc            bf-cfb            bf-ecb            bf-ofb            
camellia-128-cbc  camellia-128-ecb  camellia-192-cbc  camellia-192-ecb  
camellia-256-cbc  camellia-256-ecb  cast              cast-cbc          
cast5-cbc         cast5-cfb         cast5-ecb         cast5-ofb         
chacha            des               des-cbc           des-cfb           
des-ecb           des-ede           des-ede-cbc       des-ede-cfb       
des-ede-ofb       des-ede3          des-ede3-cbc      des-ede3-cfb      
des-ede3-ofb      des-ofb           des3              desx              
rc2               rc2-40-cbc        rc2-64-cbc        rc2-cbc           
rc2-cfb           rc2-ecb           rc2-ofb           rc4               
rc4-40            

blimp@weareribbitpmmes-MacBook-Pro ~ % openssl asn1parse
Error: offset too large
blimp@weareribbitpmmes-MacBook-Pro ~ % man openssl

     -md5 | -sha1
           The digest to use.  This affects any signing or display option that
           uses a message digest, such as the -fingerprint, -signkey, and -CA
           options.  If not specified, MD5 is used.  SHA1 is always used with
           DSA keys.

     -out file
           The output file to write to, or standard output if none is speci-
           fied.

     -outform der | net | pem
           The output format.

     -passin arg
           The key password source.

     The following are x509 display options:

     -C    Output the certificate in the form of a C source file.

     -certopt option
           Customise the output format used with -text, either using a list of
           comma-separated options or by specifying -certopt multiple times.
           The default behaviour is to print all fields.  The options are as
           follows:

                 ca_default     Equivalent to no_issuer, no_pubkey, no_header,
                                no_version, no_sigdump, and no_signame.
                 compatible     Equivalent to no output options at all.
                 ext_default    Print unsupported certificate extensions.
                 ext_dump       Hex dump unsupported extensions.
                 ext_error      Print an error message for unsupported cer-
                                tificate extensions.
                 ext_parse      ASN.1 parse unsupported extensions.
                 no_aux         Do not print certificate trust information.
                 no_extensions  Do not print X509V3 extensions.
                 no_header      Do not print header (Certificate and Data)
                                information.
                 no_issuer      Do not print the issuer name.
                 no_pubkey      Do not print the public key.
                 no_serial      Do not print the serial number.
                 no_sigdump     Do not give a hexadecimal dump of the certifi-
                                cate signature.
                 no_signame     Do not print the signature algorithm used.
                 no_subject     Do not print the subject name.
                 no_validity    Do not print the notBefore and notAfter
                                (validity) fields.
                 no_version     Do not print the version number.

     -dates
           Print the start and expiry date of a certificate.

     -email
           Output the email addresses, if any.

     -enddate
           Print the expiry date of the certificate; that is, the notAfter
           date.

     -fingerprint
           Print the digest of the DER-encoded version of the whole certifi-
           cate.
:
